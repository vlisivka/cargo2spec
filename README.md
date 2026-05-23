# cargo2spec

Create RPM Spec files for `cargo install`.

Usage: `cargo2spec CARGO_PACKAGE_NAME`

Then build RPM package from generated .spec file using command 
`rpmbuild -ba NAME.spec` , then grab binary RPM file from
`$HOME/rpmbuild/RPMS/x86_64/` directory.

To be more secure and to check dependencies, use `mock` or a similar
tool to build RPM package in a chroot.
