[![Stories in Ready](https://badge.waffle.io/Baitai/baitaidb.png?label=ready&title=Ready)](https://waffle.io/Baitai/baitaidb)
# BaitaiDB

BaitaiDB is the media tracker that anyone can edit.

## Features

- Media Tracking
  - BaitaiDB makes it easy to record, track, and share your favourite
  media - be it movies, TV shows, books, and more - all in one place.
  - Designed for the mobile web, BaitaiDB is the only tool you will need
  to track your media.  No more 3rd-party applications to access your
  data; BaitaiDB is available on all of your devices through your
  preferred browser.
- Community Editing
  - Inspired by the success of community-driven, collaborative efforts like
  Wikipedia and GitHub, BaitaiDB relies on the community for the latest
  information to keep entries up to date.
  - Contribute to editing media information, staff, character bios, and more.
  Help improve entries by contributing to the community-maintained database.
- User Customization
  - Customize list layouts and display information to highlight whatever
  is most important to you.
  - The minimal UI shows all the information that is important
  to you at a glance, but also enables easy ways to see complete media
  information.
- Updates
  - Want to be reminded when the next installment of your favourite series
 is released?  BaitaiDB makes it simple to set reminders for
 individual media, whole media types, or your entire list.
  - And we'll send you email updates to keep you in the loop, no matter
  where you are.
- User Reviews
  - Absolutely loved that movie you just watched? Think that top
  best-seller is over-priced?  Let the community know by writing a review!
  - Explore reviews and ratings from the community to find out what
  people are talking about.  Browse popular media by category, ratings,
  user votes, and more.
- Media Collection
  - Whether you already have a massive media collection or are just
  starting out, BaitaiDB makes it easy to organize your collection.
  - Sort and search your entire collection using detailed, editable
  tags, or create your own custom tag organization system.

### Stretch Goal Features

- RESTful API

## Contributing

Found a bug?  Have a feature you'd like to see implemented?  [Create an issue](https://github.com/Baitai/baitaidb/issues)!

Want to contribute to BaitaiDB's development?  We welcome [pull requests](https://github.com/Baitai/baitaidb/pulls)!

### Development

#### Requirements

##### The Code

Get the application source straight from GitHub:

```sh
git clone https://github.com/Baitai/baitaidb.git
cd baitaidb
```

##### Database

We use [PostgreSQL](http://www.postgresql.org/) as our data store.

On OS X, install PostgreSQL with Homebrew:

```sh
brew upgrade && brew update && brew cleanup
brew install postgresql
```

Installation instructions for other platforms are available in the [PostgreSQL docs](http://www.postgresql.org/download/).

Once PostgreSQL is installed and available on your `PATH`, create the development database
if it does not already exist:

```sh
createdb baitai_development
```

##### Ruby

- Ruby >= v`2.2.0`
- [Bundler](http://bundler.io/)
- [Foreman](https://github.com/ddollar/foreman)
  - `gem install foreman`

#### Installation & Setup

Install the application dependencies with

```sh
bundle install
```

Duplicate `.env.example` and rename it to `.env`.

```sh
mv .env.example .env
```

This file is used to set our development environment variables with the `dotenv-rails`
gem so we don't pollute the system environment.

#### Running the Application

Start the application server with

```sh
foreman start
```

Navigate to [localhost:3000](http://localhost:3000) and start hacking on the code.

## License

Copyright (c) 2015 Stuart Crust ([@OnAzureWings](https://github.com/OnAzureWings)).
All rights reserved.
