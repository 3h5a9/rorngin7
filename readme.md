Rails 7 One click Starter Template With Bootstrap 5 & Devise

### Instruction

- Download the repo by clone it.

- Go inside the `rorngin` folder and open terminal.

- Run the following command.

### For Postgresql
****
    `rails new appname -d postgresql -c bootstrap -m railsngin.rb `

### Update routes.rb
****
    namespace :admin do
      get '/', to: 'dashboard#index'
    end

### add custom stylesheet
****
    Go to 
    
    `app/assets/stylesheets/application.bootstrap.scss`
    
    and add

    @import 'app.scss';

***
***
### If got error in signup or sign out

  **Undefined method 'user_url'**

    Add `:turbo_stream` as a navigational format. 
    
  This line goes in `config/initializers/devise.rb`.

  uncomment the following line and add as follows
  
    config.navigational_formats = ['*/*', :html, :turbo_stream]

***
***    

### Run server
  we can run either 

  `./bin/dev` 
  
**** Or

  `rails s` 
  is going to shart the server on localhost with port 3000 as follows

  `localhost:3000`
  
  or
  
  `127.0.0.1:3000`

****


### Included
---
- fontawesome-free: "^6.0.0"
- @hotwired/stimulus: "^3.0.1"
- @hotwired/turbo-rails: "^7.1.1"
- @popperjs/core: "^2.11.2"
- bootstrap: "^5.1.3"
- esbuild: "^0.14.20"
- sass: "^1.49.7"
- Devise (Latest)