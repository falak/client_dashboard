# Project Title

This is part of a code challenge. It's a basic rails application with the following Models: Company, Employee,
PartnerCompany, Contractor and Client

- Authentication;
- Simple UI with bootstrap
- CRUD for all models

##	Note

I have also implemented an employee export function for generating the employees xls file. The function is available on employees page.

Create Employees in bulk function needs two params. The company_id and no of dummy employees to be created. I could not associate clients in bulk insert because rails insert_all method returning param is not supported in sqllite. So i could not get the ids of employees being created.

Import Employeees function performance can also be improved by using the same function but due to time constraints i could not do that. 

Error handling in import function is done right now by just raising exceptions. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Changes needed to upgrade Ruby to version 3.0+ and Rails to version 6.0+

Sqlite3 version 1.3.13 is not comptiable with ruby 3.0+, so please upgrade to version 1.4+ is a must otherwise bundle install command will give an error about sqlite3 gem installation.

To upgrade rails to 6.0+, I have just changed the version in Gemfile to 6.1.4 and run command

```
$ bundle update
```

# More Info about upgrading Ruby on Rails is available on the following website:

https://edgeguides.rubyonrails.org/upgrading_ruby_on_rails.html

### Ruby and Rails version

* 3.0.1
* 6.1.4


### Installing

Clone git repository and run bundle install:

```
$ git clone git@github.com:falak/client_dashboard.git
$ bundle install
```

Set up the database:

```
$ rails db:setup
```

Run the rails server:

```
$ rails s
```



## License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details

