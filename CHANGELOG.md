# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).
This file adheres to [Keep a changelog](http://keepachangelog.com/).

## [1.1.2] - 2015-03-01
### Fixed
- Allow symbols to fix incorrect enforcement of strings for SQL columnn names
- Accept anything responding to `to_a` to fix inability to pass ActiveRecord associations (arrays) (as opposed to relations) to `QueryResult`

## [1.1.0] - 2015-03-01 (initial Gem release)
### Added
- Averages (`avg_daily`, `avg_weekly`, `avg_monthly`)

### Fixed
- Adjust the core `method_missing` to be included in `ActiveRecord::Relation` in addition to `ActiveRecord::Base` to fix running these functions on scoped ActiveRecord queries
- Correct inflector so *_daily methods stop raising exception

### Changed
- Gemified project