# Connorsan-Resson-1.0
Programming for a preschooler.


#!/usr/bin/perl

use strict; 
use warnings;

my @heroes = ('SUPERMAN', 'CATWOMAN', 'BATMAN', 'FLASH', 'GAMBIT', 'JOKER');

@heroes = sort { $a cmp $b } map { lc($_) } grep { !/JOKER/ } @heroes;

print @heroes;
