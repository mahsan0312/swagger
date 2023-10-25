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


