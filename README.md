* ...
# swagger
Simple practice for swagger api.
rails new swagger-demo --api
rails generate model Pet name photo_url status
rails generate scaffold_controller api/v1/pets
Add rswag gem in your gemfile
bundle install
rails generate rspec:install

rails g rswag:install
generate  rswag:specs:install
       rails  generate rswag:specs:install
      create  spec/swagger_helper.rb
    generate  rswag:api:install
       rails  generate rswag:api:install
      create  config/initializers/rswag_api.rb
       route  mount Rswag::Api::Engine => '/api-docs'
    generate  rswag:ui:install
       rails  generate rswag:ui:install
      create  config/initializers/rswag_ui.rb
       route  mount Rswag::Ui::Engine => '/api-docs'

rake rswag:specs:swaggerize


The basic Dockerfile commands are:

FROM: defines what image to start from. We’ll use the official Ruby image as a starting point.
ARG: specifies build-time argument variables. If your workstation is running Linux, the user and group ids should match between the host and the docker container.
RUN: executes commands inside the container. In the example, we use it to create a user and group and then to install the Rails gems.
ENV: defines environment variables.
WORKDIR: changes the current directory inside the container.
USER: changes the active user inside the container.
CMD: defines the program to run when the container starts.
