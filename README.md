## stabilized/ClojureScript

stabilized/ClojureScript (or "s/cljs") is a distribution (*not* a
fork) of [ClojureScript](https://github.com/clojure/clojurescript)
with an emphasis on stability.  Release versions of s/cljs have
semantic meaning.

## Dependency information

Releases are deployed to
[Clojars](https://clojars.org/stabilized/clojurescript)

Latest stable release: 1.0.0 (based on [ClojureScript
0.0-2843](https://github.com/clojure/clojurescript/tree/r2843))

* [All released versions](https://clojars.org/stabilized/clojurescript)

[Leiningen](http://github.com/technomancy/leiningen/) and [Boot](http://boot-clj.com/) dependency information:

```
[stabilized/clojurescript "1.0.0"]
```

[Maven](http://maven.apache.org) dependency information:

```
<dependency>
  <groupId>stabilized</groupId>
  <artifactId>clojurescript</artifactId>
  <version>1.0.0</version>
</dependency>
```

## Rationale

We are grateful for ClojureScript and happy with how it works and is
developed.  We are less than happy with the breakneck pace of its
releases.  Our applications are particularly sensitive to our tools,
and our tools are particularly sensitive to ClojureScript's
implementation.  We have been unable to comfortably both use and
maintain our tools while also developing our applications in the face
of sometimes-weekly, sometimes-breaking ClojureScript releases.

This distribution is our effort to mediate for ourselves the pace of
upstream development as close to the root as possible, instead of
trying to do so across all of our tools and applications.  We tried,
but just don't have the time.

We invite you to use s/cljs, but also encourage you to keep using
ClojureScript proper if its quicker pace is more to your liking.
We're all on the same team!

## Release Methodology

Given a version number MAJOR.MINOR.PATCH, we will increment the:

1. MAJOR version when there are user facing, incompatible language
   changes,
2. MINOR version when there are tool-author facing, incompatible API
   changes (such as to the compiler API),
3. PATCH version when there are backwards-compatible bug fixes or
   enhancements.

* **Users** are those end-users using ClojureScript indirectly through
  some number of tools to write applications.
* **Tool-authors** are those developers who depend on internal
  ClojureScript APIs in order to develop and maintain tools that adapt
  ClojureScript to a particular development scenario, style, or
  environment.

We will regularly and selectively:

* Merge enhancements and bug fixes from upstream and increment the version number accordingly, and
* tag and deploy these new release versions to Clojars.

We will make every effort to avoid divergent changes because we are a
distribution, not a fork.  All development on s/cljs should happen
indirectly, upstream, in mainline ClojureScript.

## Helping and Contributing

We are happy to receive feedback and questions particular to s/cljs as
[Issues](https://github.com/stabilized/clojurescript/issues) in this
repository.  Otherwise, you may consider:

* Contacting the maintainers, [Alan Dipert](http://tailrecursion.com/~alan/index.cgi/index) and [Micha Niskin](http://micha.github.io/) directly, or
* interacting with other s/cljs users in [the `#hoplon` channel on freenode IRC](http://webchat.freenode.net/?channels=hoplon).

If you are interested in contributing code, or to report bugs
applicable also to ClojureScript, please consult the [ClojureScript
README](https://github.com/clojure/clojurescript).

## License

This distribution is licensed the same ClojureScript --
[EPL](https://www.eclipse.org/legal/epl-v10.html) -- and does not and
will not ever include contributions from anyone who has not [submitted
a Clojure project Contributor Agreement
(CA)](http://clojure.org/contributing).

    Copyright (c) Alan Dipert & Micha Niskin. All rights reserved. The use and
    distribution terms for this software are covered by the Eclipse
    Public License 1.0 (http://opensource.org/licenses/eclipse-1.0.php)
    which can be found in the file epl-v10.html at the root of this
    distribution. By using this software in any fashion, you are
    agreeing to be bound by the terms of this license. You must
    not remove this notice, or any other, from this software.