## You need

* **Ruby 2.0**
    * (includes RubyGems in standard library)
* **Bundler** http://bundler.io
* **Rails 4.0** (!) http://rubyonrails.org


## How to...

### Setup

    $ git clone https://github.com/PoornimaC/rss-feed-test
    $ cd rss-feed-test
    $ bundle install
    $ rake db:setup
    $ rails server
    $ http://localhost:3000
    
### Update feeds

Admin users can trigger manual updates from the web interface. The updating is done by a *rake* task, however, so you can get **automatic updates** by scheduling

    $ rake update_active_feeds
    
to run regularly in the application dir.

