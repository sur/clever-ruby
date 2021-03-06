# clever-ruby

Clever - the Ruby gem for the Clever API

The Clever API

This SDK is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.2.0
- Package version: 1.2.0
- Build package: io.swagger.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build clever-ruby.gemspec
```

Then either install the gem locally:

```shell
gem install ./clever-ruby-1.2.0.gem
```
(for development, run `gem install --dev ./clever-ruby-1.2.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'clever-ruby', '~> 1.2.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'clever-ruby', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:
```ruby
# Load the gem
require 'clever-ruby'

# Setup authorization
Clever.configure do |config|
  # Configure OAuth2 access token for authorization: oauth
  config.access_token = 'YOUR ACCESS TOKEN'
end

api_instance = Clever::DataApi.new

id = "id_example" # String | 


begin
  result = api_instance.get_contact(id)
  p result
rescue Clever::ApiError => e
  puts "Exception when calling DataApi->get_contact: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *https://api.clever.com/v1.2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*Clever::DataApi* | [**get_contact**](docs/DataApi.md#get_contact) | **GET** /contacts/{id} | 
*Clever::DataApi* | [**get_contacts**](docs/DataApi.md#get_contacts) | **GET** /contacts | 
*Clever::DataApi* | [**get_contacts_for_student**](docs/DataApi.md#get_contacts_for_student) | **GET** /students/{id}/contacts | 
*Clever::DataApi* | [**get_district**](docs/DataApi.md#get_district) | **GET** /districts/{id} | 
*Clever::DataApi* | [**get_district_admin**](docs/DataApi.md#get_district_admin) | **GET** /district_admins/{id} | 
*Clever::DataApi* | [**get_district_admins**](docs/DataApi.md#get_district_admins) | **GET** /district_admins | 
*Clever::DataApi* | [**get_district_for_school**](docs/DataApi.md#get_district_for_school) | **GET** /schools/{id}/district | 
*Clever::DataApi* | [**get_district_for_section**](docs/DataApi.md#get_district_for_section) | **GET** /sections/{id}/district | 
*Clever::DataApi* | [**get_district_for_student**](docs/DataApi.md#get_district_for_student) | **GET** /students/{id}/district | 
*Clever::DataApi* | [**get_district_for_student_contact**](docs/DataApi.md#get_district_for_student_contact) | **GET** /contacts/{id}/district | 
*Clever::DataApi* | [**get_district_for_teacher**](docs/DataApi.md#get_district_for_teacher) | **GET** /teachers/{id}/district | 
*Clever::DataApi* | [**get_district_status**](docs/DataApi.md#get_district_status) | **GET** /districts/{id}/status | 
*Clever::DataApi* | [**get_districts**](docs/DataApi.md#get_districts) | **GET** /districts | 
*Clever::DataApi* | [**get_grade_levels_for_teacher**](docs/DataApi.md#get_grade_levels_for_teacher) | **GET** /teachers/{id}/grade_levels | 
*Clever::DataApi* | [**get_school**](docs/DataApi.md#get_school) | **GET** /schools/{id} | 
*Clever::DataApi* | [**get_school_admin**](docs/DataApi.md#get_school_admin) | **GET** /school_admins/{id} | 
*Clever::DataApi* | [**get_school_admins**](docs/DataApi.md#get_school_admins) | **GET** /school_admins | 
*Clever::DataApi* | [**get_school_for_section**](docs/DataApi.md#get_school_for_section) | **GET** /sections/{id}/school | 
*Clever::DataApi* | [**get_school_for_student**](docs/DataApi.md#get_school_for_student) | **GET** /students/{id}/school | 
*Clever::DataApi* | [**get_school_for_teacher**](docs/DataApi.md#get_school_for_teacher) | **GET** /teachers/{id}/school | 
*Clever::DataApi* | [**get_schools**](docs/DataApi.md#get_schools) | **GET** /schools | 
*Clever::DataApi* | [**get_schools_for_school_admin**](docs/DataApi.md#get_schools_for_school_admin) | **GET** /school_admins/{id}/schools | 
*Clever::DataApi* | [**get_section**](docs/DataApi.md#get_section) | **GET** /sections/{id} | 
*Clever::DataApi* | [**get_sections**](docs/DataApi.md#get_sections) | **GET** /sections | 
*Clever::DataApi* | [**get_sections_for_school**](docs/DataApi.md#get_sections_for_school) | **GET** /schools/{id}/sections | 
*Clever::DataApi* | [**get_sections_for_student**](docs/DataApi.md#get_sections_for_student) | **GET** /students/{id}/sections | 
*Clever::DataApi* | [**get_sections_for_teacher**](docs/DataApi.md#get_sections_for_teacher) | **GET** /teachers/{id}/sections | 
*Clever::DataApi* | [**get_student**](docs/DataApi.md#get_student) | **GET** /students/{id} | 
*Clever::DataApi* | [**get_student_for_contact**](docs/DataApi.md#get_student_for_contact) | **GET** /contacts/{id}/student | 
*Clever::DataApi* | [**get_students**](docs/DataApi.md#get_students) | **GET** /students | 
*Clever::DataApi* | [**get_students_for_school**](docs/DataApi.md#get_students_for_school) | **GET** /schools/{id}/students | 
*Clever::DataApi* | [**get_students_for_section**](docs/DataApi.md#get_students_for_section) | **GET** /sections/{id}/students | 
*Clever::DataApi* | [**get_students_for_teacher**](docs/DataApi.md#get_students_for_teacher) | **GET** /teachers/{id}/students | 
*Clever::DataApi* | [**get_teacher**](docs/DataApi.md#get_teacher) | **GET** /teachers/{id} | 
*Clever::DataApi* | [**get_teacher_for_section**](docs/DataApi.md#get_teacher_for_section) | **GET** /sections/{id}/teacher | 
*Clever::DataApi* | [**get_teachers**](docs/DataApi.md#get_teachers) | **GET** /teachers | 
*Clever::DataApi* | [**get_teachers_for_school**](docs/DataApi.md#get_teachers_for_school) | **GET** /schools/{id}/teachers | 
*Clever::DataApi* | [**get_teachers_for_section**](docs/DataApi.md#get_teachers_for_section) | **GET** /sections/{id}/teachers | 
*Clever::DataApi* | [**get_teachers_for_student**](docs/DataApi.md#get_teachers_for_student) | **GET** /students/{id}/teachers | 
*Clever::EventsApi* | [**get_event**](docs/EventsApi.md#get_event) | **GET** /events/{id} | 
*Clever::EventsApi* | [**get_events**](docs/EventsApi.md#get_events) | **GET** /events | 
*Clever::EventsApi* | [**get_events_for_school**](docs/EventsApi.md#get_events_for_school) | **GET** /schools/{id}/events | 
*Clever::EventsApi* | [**get_events_for_school_admin**](docs/EventsApi.md#get_events_for_school_admin) | **GET** /school_admins/{id}/events | 
*Clever::EventsApi* | [**get_events_for_section**](docs/EventsApi.md#get_events_for_section) | **GET** /sections/{id}/events | 
*Clever::EventsApi* | [**get_events_for_student**](docs/EventsApi.md#get_events_for_student) | **GET** /students/{id}/events | 
*Clever::EventsApi* | [**get_events_for_teacher**](docs/EventsApi.md#get_events_for_teacher) | **GET** /teachers/{id}/events | 


## Documentation for Models

 - [Clever::BadRequest](docs/BadRequest.md)
 - [Clever::Credentials](docs/Credentials.md)
 - [Clever::District](docs/District.md)
 - [Clever::DistrictAdmin](docs/DistrictAdmin.md)
 - [Clever::DistrictAdminResponse](docs/DistrictAdminResponse.md)
 - [Clever::DistrictAdminsResponse](docs/DistrictAdminsResponse.md)
 - [Clever::DistrictObject](docs/DistrictObject.md)
 - [Clever::DistrictResponse](docs/DistrictResponse.md)
 - [Clever::DistrictStatus](docs/DistrictStatus.md)
 - [Clever::DistrictStatusResponse](docs/DistrictStatusResponse.md)
 - [Clever::DistrictStatusResponses](docs/DistrictStatusResponses.md)
 - [Clever::DistrictsResponse](docs/DistrictsResponse.md)
 - [Clever::Event](docs/Event.md)
 - [Clever::EventResponse](docs/EventResponse.md)
 - [Clever::EventsResponse](docs/EventsResponse.md)
 - [Clever::GradeLevelsResponse](docs/GradeLevelsResponse.md)
 - [Clever::InternalError](docs/InternalError.md)
 - [Clever::Location](docs/Location.md)
 - [Clever::Name](docs/Name.md)
 - [Clever::NotFound](docs/NotFound.md)
 - [Clever::Principal](docs/Principal.md)
 - [Clever::School](docs/School.md)
 - [Clever::SchoolAdmin](docs/SchoolAdmin.md)
 - [Clever::SchoolAdminObject](docs/SchoolAdminObject.md)
 - [Clever::SchoolAdminResponse](docs/SchoolAdminResponse.md)
 - [Clever::SchoolAdminsResponse](docs/SchoolAdminsResponse.md)
 - [Clever::SchoolObject](docs/SchoolObject.md)
 - [Clever::SchoolResponse](docs/SchoolResponse.md)
 - [Clever::SchoolsResponse](docs/SchoolsResponse.md)
 - [Clever::Section](docs/Section.md)
 - [Clever::SectionObject](docs/SectionObject.md)
 - [Clever::SectionResponse](docs/SectionResponse.md)
 - [Clever::SectionsResponse](docs/SectionsResponse.md)
 - [Clever::Student](docs/Student.md)
 - [Clever::StudentContact](docs/StudentContact.md)
 - [Clever::StudentContactObject](docs/StudentContactObject.md)
 - [Clever::StudentContactResponse](docs/StudentContactResponse.md)
 - [Clever::StudentContactsForStudentResponse](docs/StudentContactsForStudentResponse.md)
 - [Clever::StudentContactsResponse](docs/StudentContactsResponse.md)
 - [Clever::StudentObject](docs/StudentObject.md)
 - [Clever::StudentResponse](docs/StudentResponse.md)
 - [Clever::StudentsResponse](docs/StudentsResponse.md)
 - [Clever::Teacher](docs/Teacher.md)
 - [Clever::TeacherObject](docs/TeacherObject.md)
 - [Clever::TeacherResponse](docs/TeacherResponse.md)
 - [Clever::TeachersResponse](docs/TeachersResponse.md)
 - [Clever::Term](docs/Term.md)
 - [Clever::DistrictsCreated](docs/DistrictsCreated.md)
 - [Clever::DistrictsDeleted](docs/DistrictsDeleted.md)
 - [Clever::DistrictsUpdated](docs/DistrictsUpdated.md)
 - [Clever::SchooladminsCreated](docs/SchooladminsCreated.md)
 - [Clever::SchooladminsDeleted](docs/SchooladminsDeleted.md)
 - [Clever::SchooladminsUpdated](docs/SchooladminsUpdated.md)
 - [Clever::SchoolsCreated](docs/SchoolsCreated.md)
 - [Clever::SchoolsDeleted](docs/SchoolsDeleted.md)
 - [Clever::SchoolsUpdated](docs/SchoolsUpdated.md)
 - [Clever::SectionsCreated](docs/SectionsCreated.md)
 - [Clever::SectionsDeleted](docs/SectionsDeleted.md)
 - [Clever::SectionsUpdated](docs/SectionsUpdated.md)
 - [Clever::StudentcontactsCreated](docs/StudentcontactsCreated.md)
 - [Clever::StudentcontactsDeleted](docs/StudentcontactsDeleted.md)
 - [Clever::StudentcontactsUpdated](docs/StudentcontactsUpdated.md)
 - [Clever::StudentsCreated](docs/StudentsCreated.md)
 - [Clever::StudentsDeleted](docs/StudentsDeleted.md)
 - [Clever::StudentsUpdated](docs/StudentsUpdated.md)
 - [Clever::TeachersCreated](docs/TeachersCreated.md)
 - [Clever::TeachersDeleted](docs/TeachersDeleted.md)
 - [Clever::TeachersUpdated](docs/TeachersUpdated.md)


## Documentation for Authorization


### oauth

- **Type**: OAuth
- **Flow**: accessCode
- **Authorization URL**: https://clever.com/oauth/authorize
- **Scopes**: N/A

## Previous Versions

The current client support v1.2 of the API. For v1.1 please use:

https://rubygems.org/gems/clever-ruby/versions/0.14.0
https://github.com/Clever/clever-ruby/tree/0.14


## Updating the Library

1. Git clone swagger-codegen (https://github.com/swagger-api/swagger-codegen)

2. Git clone Clever's swagger-api repo (https://github.com/Clever/swagger-api)

3. Run this command in the swagger-codegen repo
```
java -jar modules/swagger-codegen-cli/target/swagger-codegen-cli.jar generate -i $PATH_TO_SWAGGER_API_REPO/v1.2-client.yml -c $PATH_TO_THIS_REPO/override/config.json -l ruby -o $PATH_TO_THIS_REPO
```

4. Run `make build` to copy over the override files


## Publishing

Signup to rubygems.org if you don't already have an account, and ask one of the gem [owners](https://rubygems.org/gems/clever-ruby) to add you as an owner. You'll be prompted to log in from the command line when you push the gem, if you aren't already logged in.

To add a new owner, you need to be an owner, then run this command: `gem owner clever-ruby -a <emailaddress>`

1. Update `CHANGELOG.md`
1. `gem build clever-ruby.gemspec`
1. `gem push clever-ruby-X.Y.Z.gem`