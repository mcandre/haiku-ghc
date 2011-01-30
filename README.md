haiku-ghc - Build GHC on Haiku

REQUIREMENTS

 - [Git](http://www.haiku-os.org/blog/nielx/2008-04-21/git_for_haiku_1)

TIPS

 - Haiku does not come with vi or vim. Use nano instead.

INSTRUCTIONS

1. Get the GHC source.

    ~> wget http://www.haskell.org/ghc/dist/7.0.3/ghc-7.0.3-src.tar.bz2
    ~> tar xvf ghc-7.0.3-src.tar.bz2
    ~> cd ghc-7.0.3/

2. Edit the Perl boot script to use "perl" instead of "/usr/bin/perl".

    ~> sed 's/\/usr\/bin\///' <boot >boot.new
    ~> mv boot.new boot

3. Run the Perl boot script.

    ~> perl boot
    Creating libraries
    ...
