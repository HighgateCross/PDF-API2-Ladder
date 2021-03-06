# NAME

PDF::API2::Ladder - Creates PDFs a line at a time, much like the rungs on a ladder.

# SYNOPSIS

    use PDF::API2::Ladder;

    # Create a new PDF::Ladder Object
    $pdf = PDF::Ladder->new(   font_size       => $font_size,
                               lead            => $lead,
                               font            => 'Georgia',
                               show_margins    => $show_margins,
                               margin_top      => .5/in,
                               margin_bottom   => .5/in,
                               line_height     => $line_height);

    # Create a Rung at the top of the page (since its the first) that is center.
    $pdf->add_rung("An Amazing Play", align  => 'center');
    # Create a Rung underneath that, which is not centered
    $pdf->add_rung("Actor1: 'To be or not 2 B. That is the answer!');

# DESCRIPTION

PDF::API2::Ladder is a simplified way of creating PDFs using the awesome module PDF::API2. PDF::API2::Ladder builds PDFs in a top down fashion much like rungs on a ladder. The exception to the rung style is what is called a Blob. Blobs do not have a set height and adapt to their contents height instead. New pages are created automatically when a rung or blob goes off the end of the page.

# METHODS

    TODO

# AUTHOR

Sean Zellmer <sean@lejeunerenard.com>

# COPYRIGHT

Copyright 2013- Sean Zellmer

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

- [PDF::API2](http://search.cpan.org/perldoc?PDF::API2)
- [PDF::API2::Simple](http://search.cpan.org/perldoc?PDF::API2::Simple)
