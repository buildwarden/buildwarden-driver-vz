# buildwarden-driver-vz

The BuildWarden vz driver: one driver, as its own binary that speaks the driver contract (seam 9), built on the kit.

This repository is one component of BuildWarden's componentization program,
which splits the project into components that meet only at written seams. The
umbrella design says where the program ends, which component holds what, and
the order of the phases:

- [Componentization](https://github.com/buildwarden/buildwarden/blob/main/docs/design/componentization.md)
- [Program north star](https://github.com/buildwarden/buildwarden/blob/main/docs/design/program-north-star.md)
- The seam specifications and their conformance suites:
  [`buildwarden/buildwarden-specs`](https://github.com/buildwarden/buildwarden-specs)

The repository is empty until its phase of the program starts. Work lands on
the program trunk, `program/componentization`, by merged pull requests only, and
reaches `main` in the program's landing merge.

## License

Apache License 2.0; see [LICENSE](LICENSE).
