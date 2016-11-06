# frp

A _Scala Functional Reactive Programming_ (_FRP_) library, initially based upon
_[Sodium](https://github.com/SodiumFRP/sodium)_. It is intended for _Scala_ developers writing _FRP_-driven applications
as well as _[Facsimile](http://facsim.org/)_ simulation model developers.

# Motivation

_frp_ was inspired by the excellent _[Scala.React](https://github.com/ingoem/scala-react)_ and
_[Sodium](https://github.com/SodiumFRP/sodium)_ projects. Unfortunately, _Scala.React_ has yet to be released under an
open source license, while the primary focus of _Sodium_ development is the _Java_ language1. (There is an official
_Scala_ port of _Sodium_, but it is relatively immature; furthermore, we feel it likely that it would make more sense
for the _Sodium_ project to support a single _JVM_-flavor of _Sodium_ (covering languages such as _Clojure_, _Kotlin_,
_Scala_, etc. Right now, the _Sodium_ project seems to be supporting a number of different languages in a rather
uncontrolled manner.) As a language designed for _functional programming_, we feel that a native _Scala FRP_ library
can be simpler and easier to maintain than a library written in _Java_.

Another minor point is that we feel that certain of _Sodium_'s class and primitive names are _inconsistent_ with _Scala_
conventions, or have associations that would cause confusion for simulation developers. Instead, _frp_ strives to
replicate the _domain-specific language_ features and _API_ of _Scala.React_.

_frp_ is the framework used by _Facsimile_ for handling simulation, _graphical user interface_ (_GUI_) and other event
sources.