# NAME

Zing::Zang - Process Implementation

# ABSTRACT

Process Implementation

# SYNOPSIS

    use Zing::Zang;

    my $zang = Zing::Zang->new(
      on_perform => sub {
        my ($self) = @_;

        $self->{performed}++
      }
    );

    # $zang->execute;

# DESCRIPTION

This package provides a standard [Zing::Process](https://metacpan.org/pod/Zing%3A%3AProcess) which uses callbacks and
doesn't need to be subclassed. It supports providing the standard process
`perform` method as `on_perform` and `receive` method as `on_receive` which
operate as expected.

# INHERITS

This package inherits behaviors from:

[Zing::Process](https://metacpan.org/pod/Zing%3A%3AProcess)

# LIBRARIES

This package uses type constraints from:

[Zing::Types](https://metacpan.org/pod/Zing%3A%3ATypes)

# ATTRIBUTES

This package has the following attributes:

## on\_perform

    on_perform(Maybe[CodeRef])

This attribute is read-only, accepts `(Maybe[CodeRef])` values, and is optional.

## on\_receive

    on_receive(Maybe[CodeRef])

This attribute is read-only, accepts `(Maybe[CodeRef])` values, and is optional.

# AUTHOR

Al Newkirk, `awncorp@cpan.org`

# LICENSE

Copyright (C) 2011-2019, Al Newkirk, et al.

This is free software; you can redistribute it and/or modify it under the terms
of the The Apache License, Version 2.0, as elucidated in the ["license
file"](https://github.com/cpanery/zing-zang/blob/master/LICENSE).

# PROJECT

[Wiki](https://github.com/cpanery/zing-zang/wiki)

[Project](https://github.com/cpanery/zing-zang)

[Initiatives](https://github.com/cpanery/zing-zang/projects)

[Milestones](https://github.com/cpanery/zing-zang/milestones)

[Contributing](https://github.com/cpanery/zing-zang/blob/master/CONTRIBUTE.md)

[Issues](https://github.com/cpanery/zing-zang/issues)
