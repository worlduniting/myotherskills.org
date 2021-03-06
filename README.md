# MyOtherSkills.org

[Demo](http://myotherskills.herokuapp.com/)

MyOtherSkills.org is a place to tell the world about EVERYTHING you can do, not just your resume. Are you a Doctor who can juggle? Are you a carpentar who plays piano? Are you a professional yodaller who knows how to read ancient Greek?

MyOtherSkills is a Front-end / Back-end template using HTML5 Boilerplate, Twitter Bootstrap 3, Ruby on Rails (4.0.0) Devise ( Auth ) and Ruby 2.0.0.

## Quick start

* Clone the git repo - `git clone https://github.com/blueheadpublishing/myotherskills.git`

* Run `bundle install`
* Run `rake db:migrate`


Then run your server
<pre>
rails s
</pre>

Check at [http://localhost:3000](http://localhost:3000)

## Requirements

* Rails 4
* Ruby 2.0.0
* Imagemagick (For uploading pictures)
* Vagrant (Optional)
* This app is configured to run on Heroku's Cedar Stack. More info here https://devcenter.heroku.com/articles/getting-started-with-rails4


## Features

##### [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/)

##### [Twitter Bootstrap 3](http://twitter.github.com/bootstrap/index.html)

##### [HAML Template Engine](http://haml.info/)

##### [Ruby on Rails 4.0.0](http://rubyonrails.org/)
* Devise
* Paperclip ( User profile picture )


### Databases support

* SQLite (Default)
* Postgresdb [https://github.com/hugodias/MyOtherSkills/tree/postgresdb](https://github.com/hugodias/MyOtherSkills/tree/postgresdb)


#### Vagrant
---
MyOtherSkills has a *Vagrant* file to create your own Virtual Machine for development.

To get started you need to have [Vagrant](http://www.vagrantup.com) and [Virtal Box](https://www.virtualbox.org/) instaled.

After that you just need to start your VM:
<pre>vagrant up</pre>

##### Bonus
After that you have a Ubuntu server to work, but this server isn't configured to work with rails yet! :( So i'm leaving here one virtual box image with Ruby 2.0.0 (rbenv) and Rails 4 pre-configured.

To install this server just follow this steps:

* Download the server image here: [link](https://mega.co.nz/#!Fsd0Tbrb!Ud68qgxpD9Av8VxdrVNPtCWciyh_DosXCopDWJksg4M
)
* Place the image that you downloaded in MyOtherSkills repository
* In MyOtherSkills directory run `vagrant box add MyOtherSkillsMachine ubuntuRails4Ruby2.box virtualbox`
* Run `vagrant box list` and this new machine should be in that list
* Now in `Vagrantfile` change `config.vm.box="precise32"` to `config.vm.box="MyOtherSkillsMachine"`
* To get your machine up run `vagrant up`

And its done ! Your vagrant vm now has Ruby 2.0.0 and Rails 4 ready to go.

---

## License

### Major components:

* jQuery: MIT/GPL license
* Modernizr: MIT/BSD license
* Normalize.css: Public Domain
* Twitter bootstrap: [Apache License, Version 2.0 (the "License")](http://www.apache.org/licenses/LICENSE-2.0)
* Ruby on Rails: MIT license

### Everything else:

The Unlicense (aka: public domain)


      :postgresql => {
        :config   => {
          :listen_addresses => "*",
          :port             => "5432"
        },
        :pg_hba   => [
          {
            :type   => "local",
            :db     => "postgres",
            :user   => "postgres",
            :addr   => nil,
            :method => "trust"
          },
          {
            :type   => "host",
            :db     => "all",
            :user   => "all",
            :addr   => "0.0.0.0/0",
            :method => "md5"
          },
          {
            :type   => "host",
            :db     => "all",
            :user   => "all",
            :addr   => "::1/0",
            :method => "md5"
          }
        ],
        :password => {
          :postgres => "password"
        }
      },
