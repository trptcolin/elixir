# Changelog for Elixir v1.9

## v1.9.0-dev

### 1. Enhancements

#### EEx

  * [EEx] Allow more complex mixed expression when tokenizing

#### Elixir

  * [CLI] Add support for `--boot`, `--boot-var`, `--erl-config`, `--pipe-to`, `--rpc-eval`, and `--vm-args` options
  * [File] Add `File.rename!/2`
  * [Kernel] Optimize generated code for `with` with a catch-all clause
  * [Protocol] Improve Protocol.UndefinedError messages to also include the type that was attempted to dispatch on
  * [System] Add `System.restart/0` and `System.pid/0`
  * [System] Support `SOURCE_DATE_EPOCH` for reproducible builds

#### ExUnit

  * [ExUnit.DocTest] No longer wrap doctest errors in custom exceptions. They ended-up hiding more information than showing

#### Logger

  * [Logger] Use a descentralized mode computation for Logger which allows overloads to be detect more quickly

#### Mix

  * [mix release] Add support for releases

### 2. Bug fixes

#### Elixir

  * [Kernel] Properly merge and handle docs for callbacks with multiple clauses
  * [Kernel] Guarantee reproducible builds on modules with dozens of specs
  * [Kernel] Resolve `__MODULE__` accordingly in nested `defmodule` to avoid double nesting

#### ExUnit

  * [ExUnit] Raise error if attempting to run single line tests on multiple files

#### IEx

  * [IEx] Automatically shut down IEx if we receive EOF

### 3. Soft-deprecations (no warnings emitted)

### 4. Hard-deprecations

#### Elixir

  * [CLI] Deprecate `--detached` option, use `--erl "-detached"` instead

#### Mix

  * [Mix.Project] Deprecate `Mix.Project.load_paths/1` in favor of `Mix.Project.compile_path/1`

## v1.8

The CHANGELOG for v1.8 releases can be found [in the v1.8 branch](https://github.com/elixir-lang/elixir/blob/v1.8/CHANGELOG.md).
