# NAME

Types::PerlVersion - [Perl::Version](https://metacpan.org/pod/Perl::Version) type constraint for [Type::Tiny](https://metacpan.org/pod/Type::Tiny)

# VERSION

Version 0.001

# SYNOPSIS

```perl
package MyApp::Thingie;

use Moose;
use Types::PerlVersion qw/PerlVersion/;

has version => (
    is       => 'ro',
    isa      => PerlVersion,
    coerce   => 1,
    required => 1,
);
```

# DESCRIPTION

[Types::PerlVersion](https://metacpan.org/pod/Types::PerlVersion) is a type constraint suitable for use with
[Moo](https://metacpan.org/pod/Moo)/[Moose](https://metacpan.org/pod/Moose) attributes that need to deal with version strings as
handled by [Perl::Version](https://metacpan.org/pod/Perl::Version).

## Types

This module provides the single type constraint `PerlVersion`. Coercion is
provided from `Str` and `Num` types.

# AUTHOR

Peter Mottram (SysPete), `<peter at sysnix.com>`

# BUGS

Please report any bugs found to:

[https://github.com/SysPete/p5-Types-PerlVersion/issues](https://github.com/SysPete/p5-Types-PerlVersion/issues)

# SUPPORT

You can find documentation for this module with the perldoc command.

```
perldoc Types::PerlVersion
```

You can also look for information at:

- [GitHub repository](https://github.com/SysPete/p5-Types-PerlVersion)
- [meta::cpan](https://metacpan.org/pod/Types::PerlVersion)

# SEE ALSO

If you prefer to use [MooseX::Types](https://metacpan.org/pod/MooseX::Types) then see [MooseX::Types::PerlVersion](https://metacpan.org/pod/MooseX::Types::PerlVersion)
which was the basis of this module.

# ACKNOWLEDGEMENTS

Toby Inkster for his excellent [Type::Tiny](https://metacpan.org/pod/Type::Tiny), brian d foy for [Perl::Version](https://metacpan.org/pod/Perl::Version)
and Roman F. for [MooseX::Types::PerlVersion](https://metacpan.org/pod/MooseX::Types::PerlVersion) from which I stole most of the
code for this module.

# LICENSE AND COPYRIGHT

Copyright 2015 Peter Mottram (SysPete).

This program is free software; you can redistribute it and/or modify
it under the same terms as the Perl 5 programming language system itself.
