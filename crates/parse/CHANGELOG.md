# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.4](https://github.com/paradigmxyz/solar/releases/tag/v0.1.4)

### Bug Fixes

- Windows eol lexing ([#340](https://github.com/paradigmxyz/solar/issues/340))
- [parser] Allow EVM builtins to be present in yul paths ([#336](https://github.com/paradigmxyz/solar/issues/336))

### Dependencies

- [lexer] Rewrite prefixed literal lexing ([#325](https://github.com/paradigmxyz/solar/issues/325))

### Features

- [sema] Implement receive function checks ([#321](https://github.com/paradigmxyz/solar/issues/321))
- Add span in FunctionHeader ([#318](https://github.com/paradigmxyz/solar/issues/318))
- [ast] Add spans to blocks ([#314](https://github.com/paradigmxyz/solar/issues/314))

### Miscellaneous Tasks

- [lexer] Cursor cleanup ([#338](https://github.com/paradigmxyz/solar/issues/338))

### Performance

- [lexer] Use slice::Iter instead of Chars in Cursor ([#339](https://github.com/paradigmxyz/solar/issues/339))
- [lexer] Use memchr in block_comment ([#337](https://github.com/paradigmxyz/solar/issues/337))
- [lexer] Add eat_until ([#324](https://github.com/paradigmxyz/solar/issues/324))

## [0.1.3](https://github.com/paradigmxyz/solar/releases/tag/v0.1.3)

### Bug Fixes

- [parser] Clear docs if not consumed immediatly ([#309](https://github.com/paradigmxyz/solar/issues/309))
- [parser] Named call arguments are allowed to be empty ([#283](https://github.com/paradigmxyz/solar/issues/283))
- Invalid underscores check ([#281](https://github.com/paradigmxyz/solar/issues/281))
- [parser] Typo in concatenated string literals
- [parser] Align number parsing with solc ([#272](https://github.com/paradigmxyz/solar/issues/272))
- [parser] Correct token precedence ([#271](https://github.com/paradigmxyz/solar/issues/271))
- [parser] Ignore comments in lookahead ([#267](https://github.com/paradigmxyz/solar/issues/267))
- [parser] Remove RawTokenKind::UnknownPrefix ([#260](https://github.com/paradigmxyz/solar/issues/260))
- [parser] Don't panic when parsing hex rationals ([#256](https://github.com/paradigmxyz/solar/issues/256))

### Features

- [parser] Accept non-checksummed addresses, to be validated later ([#285](https://github.com/paradigmxyz/solar/issues/285))
- [ast] Store concatenated string literals ([#266](https://github.com/paradigmxyz/solar/issues/266))
- [ast] Add span to CallArgs ([#265](https://github.com/paradigmxyz/solar/issues/265))
- Pretty printing utilities ([#264](https://github.com/paradigmxyz/solar/issues/264))
- [parser] Use impl Into<String> ([#258](https://github.com/paradigmxyz/solar/issues/258))

### Miscellaneous Tasks

- [lexer] Add tokens.capacity log
- Tweak tracing events ([#255](https://github.com/paradigmxyz/solar/issues/255))
- Revert extra changelog

### Performance

- [lexer] Deal with bytes instead of chars in Cursor ([#279](https://github.com/paradigmxyz/solar/issues/279))
- [lexer] Filter out comments again ([#269](https://github.com/paradigmxyz/solar/issues/269))
- [lexer] Double tokens capacity estimate ([#268](https://github.com/paradigmxyz/solar/issues/268))

## [0.1.2](https://github.com/paradigmxyz/solar/releases/tag/v0.1.2)

### Bug Fixes

- [parser] Glob imports require an alias ([#245](https://github.com/paradigmxyz/solar/issues/245))
- Correctly resolve try/catch scopes ([#200](https://github.com/paradigmxyz/solar/issues/200))

### Features

- Refactor FileResolver to allow custom current_dir ([#235](https://github.com/paradigmxyz/solar/issues/235))
- Parse storage layout specifiers ([#232](https://github.com/paradigmxyz/solar/issues/232))

### Miscellaneous Tasks

- Shorten Diagnostic* to Diag ([#184](https://github.com/paradigmxyz/solar/issues/184))

### Performance

- Make Token implement Copy ([#241](https://github.com/paradigmxyz/solar/issues/241))

## [0.1.1](https://github.com/paradigmxyz/solar/releases/tag/v0.1.1)

### Bug Fixes

- Add Session::enter_parallel ([#183](https://github.com/paradigmxyz/solar/issues/183))
- [parser] Accept leading dot in literals ([#151](https://github.com/paradigmxyz/solar/issues/151))
- [parser] Span of partially-parsed expressions ([#139](https://github.com/paradigmxyz/solar/issues/139))
- [parser] Ignore more doc comments ([#136](https://github.com/paradigmxyz/solar/issues/136))

### Documentation

- Add icons ([#109](https://github.com/paradigmxyz/solar/issues/109))

### Features

- Add some more Span utils ([#179](https://github.com/paradigmxyz/solar/issues/179))
- [parser] Allow doc-comments anywhere ([#154](https://github.com/paradigmxyz/solar/issues/154))
- Validate variable data locations ([#149](https://github.com/paradigmxyz/solar/issues/149))
- [parser] Recover old-style fallbacks ([#135](https://github.com/paradigmxyz/solar/issues/135))
- Make parse_semver_req public ([#114](https://github.com/paradigmxyz/solar/issues/114))

### Miscellaneous Tasks

- Remove Pos trait ([#137](https://github.com/paradigmxyz/solar/issues/137))

### Other

- Validate num. variants in enum declaration ([#120](https://github.com/paradigmxyz/solar/issues/120))
- Better error for struct without any fields ([#121](https://github.com/paradigmxyz/solar/issues/121))

### Refactor

- Re-export ast::* internal module ([#141](https://github.com/paradigmxyz/solar/issues/141))

## [0.1.0](https://github.com/paradigmxyz/solar/releases/tag/v0.1.0)

Initial release.

<!-- generated by git-cliff -->
