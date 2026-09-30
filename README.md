# libsecret

![Mirror](https://img.shields.io/badge/mirror-read--only-blue)
![Upstream](https://img.shields.io/badge/upstream-gitlab.gnome.org%2FGNOME%2Flibsecret-orange)
![License](https://img.shields.io/badge/license-LGPL--2.1-green)

> ## 🔗 Fork / mirror note
>
> This repository is a **read-only mirror** of the GNOME project:
> [`https://gitlab.gnome.org/GNOME/libsecret`](https://gitlab.gnome.org/GNOME/libsecret)
>
> - Contributions, bug reports, and merge requests go **upstream** (GitLab), not here.
> - Upstream project README, build docs, and contributing guidance are preserved
>   verbatim below.
> - No local divergences from upstream have been recorded in this mirror.
> - Nightly documentation: <https://gnome.pages.gitlab.gnome.org/libsecret/>

---

libsecret
=========

A [GObject]-based library for storing and receiving secrets. libsecret provides
a convenient wrapper around two different mechanisms: If available, secrets are
stored in the freedesktop [secret service]. Otherwise, secrets are stored in a
file that is encrypted using a master secret that was provided by the [secret
portal].

Documentation
--------

You can find the nightly documentation at https://gnome.pages.gitlab.gnome.org/libsecret/.

Building
--------

To build, test and install libsecret, you can use the following commands:

```
$ meson setup _build
$ meson compile -C _build
$ meson test -C _build
$ meson install -C _build
```

Contributing
-------------

You can browse the code, issues and more at libsecret's [GitLab repository].

If you find a bug in libsecret, please file an issue on the [issue tracker].
Please try to add reproducible steps and the relevant version of libsecret.

If you want to contribute functionality or bug fixes, please open a Merge
Request (MR). For more info on how to do this, see GitLab's [help pages on
MR's].

If libsecret is not translated in your language or you believe that the
current translation has errors, you can join one of the various translation
teams in GNOME. Translators do not commit directly to Git, but are advised to
use our separate translation infrastructure instead. More info can be found at
the [translation project Welcome page].

Releases
-------------

The release tarballs use [semantic versioning] since 0.19.0, which
basically means:

- The major version will be incremented if backward incompatible changes are added
- The minor version will be incremented if new functionality is added in a backward compatible manner
- The patch version will be incremented if only backward compatible bug fixes are added

Note that there is no stable/unstable indication in whether the minor
version number is even or odd.


[GObject]: https://developer.gnome.org/gobject/stable/
[secret service]: https://specifications.freedesktop.org/secret-service-spec/
[secret portal]: https://flatpak.github.io/xdg-desktop-portal/docs/doc-org.freedesktop.portal.Secret.html
[GitLab repository]: https://gitlab.gnome.org/GNOME/libsecret
[help pages on MR's]: https://docs.gitlab.com/ee/gitlab-basics/add-merge-request.html
[issue tracker]: https://gitlab.gnome.org/GNOME/libsecret/issues
[translation project Welcome page]: https://welcome.gnome.org/team/translation/
[semantic versioning]: https://semver.org

---

## Security

libsecret is a credential store — see the freedesktop [secret service] spec for
the protocol. Vulnerability reports go **upstream** per the GNOME security
policy; this mirror is not the right place to file them.

## License

LGPL-2.1 — see [`COPYING`](COPYING) in this repo (upstream license file).
