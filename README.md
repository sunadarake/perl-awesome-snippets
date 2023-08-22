# perl-awesome-snippets

This extension provides useful snippets for Perl programming.

It includes a wide range of snippets that aim to make certain tedious coding tasks in Perl more convenient, such as handling features and other repetitive constructs.

## How to Install

```bash
curl -fsSL https://github.com/sunadarake/perl-awesome-snippets/raw/main/perl-awesome-snippets-0.0.1.vsix > perl-awesome-snippets-0.0.1.vsix
code --install-extension  perl-awesome-snippets-0.0.1.vsix
```

## Snippets

### Feature

| Snippets | Output |
| --- | --- |
| feature | use strict; use warnings; use feature qw/ say /; use utf8; use Data::Dumper; |
| file_feature | use File::Path; use File::Basename; use File::Spec; use File::Find; use File::Temp; use File::Copy; |
| getopt_feature | use Getopt::Long qw(:config posix_default no_ignore_case gnu_compat); |

### Control

| Snippets | Output |
| --- | --- |
| if | if (condition) { #code... } |
| ife | if (condition) { #code... } else { #code... } |
| else | else { #code... } |
| elsif, elif, eif | elsif (cond) { #code... } |
| ifelif, ifelsif | if (cond) { #code... } elsif (cond) { #code... } |


### File

| Snippets | Output |
| --- | --- |
| file_get_contents | sub file_get_contents { my $file = shift; open( my $fh, "<", $file ) or die("cannot open $file"); return do { local $/; <$fh>; }; } |
| file_put_contents | sub file_put_contents { my ( $file, $content ) = @_; open( my $fh, ">", $file ) or die("cannot open $file"); print $fh $content; } |
| ropen | open( my $fh, "<", $file ) or die("cannot open $file"); |
| wopen | open( my $fh, ">", $file ) or die("cannot open $file"); |

### Subroutine

| Snippets | Output |
| --- | --- |
| fn, sub | sub ${1:sub_name} { my ${2:$item} = shift; } |
| fna, fn_, suba, sub_ | sub ${1:sub_name} { my (${2:args}) = @_; } |

### Loop

| Snippets | Output |
| --- | --- |
| while, whl | while (${1:cond}) { ${2:# code ..} } |
| unless, unl | unless (${1:cond}) { ${2:# code ..} } |
| for | for (${1:@$items}) { ${2:# code ..} } |
| forv | for my ${1:$item} (${2:@$items}) { ${3:# code ..} } |
