My Xcode code snippets
======================

There are two folders in this repository:

1. AzizLight.snippetbundle
2. CodeSnippets

The first one contains my snippets with a nice file name so that your
eyes don't bleed when you will browse them. The second one contains
the snippets with their UUID as filename (this time your eyes will
bleed!).

Installation
------------

First, you need to clone this repository:

~~~sh
% git clone https://github.com/AzizLight/Xcode-Snippets.git
~~~

Then you have two options:

1. Install the snippets using [the xcodesnippets gem](https://github.com/AzizLight/xcodesnippets)
2. Install the snippets manually

### Using the xcodesnippets gem

If you use [the xcodesnippets gem](https://github.com/AzizLight/xcodesnippets) you can just run the following command to install all of my snippets:

```sh
% xcodesnippets install-bundle AzizLight.snippetbundle
```

If you don't want to install all the snippets at once, but rather want
to install a couple of them, you can do that as well:

```sh
% cd AzizLight.snippetbundle/
% xcodesnippets install !!!.codesnippet
% xcodesnippets install ???.codesnippet
```

### Installing the snippets manually

If you want to install all the snippets manually, copy and paste this
command into your terminal (**Note that you need to be in the repository directory!**):

```sh
% cp -R CodeSnippets/* ~/Library/Developer/Xcode/UserData/CodeSnippets/
```

If you want to install only a couple of snippets, do the same but for
individual snippets:

```sh
% cp -R CodeSnippets/003C261B-E9CC-4777-B91B-46130E357951.codesnippet ~/Library/Developer/Xcode/UserData/CodeSnippets/
```

Et Voil&agrave;!

My snippets
-----------

Here is a list of the snippets I've added myself. I didn't include the other snippets in this list.

### Tasks snippets

- `!!!` in `!!!.codesnippet` and `5FF971E0-845B-4F18-932A-70FB687A1FAA.codesnippet`

```objc
// !!!: <#Note#>
```

- `???` in `???.codesnippet` and `EA231A0C-23B8-47CA-B6AF-D69367AA6C24.codesnippet`

```objc
// ???: <#Note#>
```

- `fixme` in `FIXME.codesnippet` and `2562208A-CCF4-4210-91F1-451FC812D915.codesnippet`

```objc
// FIXME: <#Note#>
```

- `todo` in `TODO.codesnippet` and `5DEC045C-4073-4EA3-BB71-488CFB930D87.codesnippet`

```objc
// TODO: <#Note#>
```

### Pre-processor directives

- `ddd` in `#define.codesnippet` and `955785AC-A3A8-41B4-AF02-4BAC8E0FDD01.codesnippet`

```objc
#define k<#constant name#> <#constant value#>
```

- `ifd` in `#if DEBUG.codesnippet` and `B981685E-B238-4A91-88A3-450712A7204C.codesnippet`

```objc
#if DEBUG
	<#whatever#>
#endif
```

- `iii` in `#import.codesnippet` and `484A4FBA-2746-4250-93C4-AAE43708BBFC.codesnippet`

```objc
#import "<#header#>.h"
```

- `mark` in `#pragma Mark.codesnippet` and `C97C64B0-19B7-44E6-AA28-6FDF064BCC15.codesnippet`

```objc
#pragma mark - <#Section#>
```

### Utility

- `arg` in `Method argument.codesnippet` and `58349CF2-81D0-4BB1-94B7-74FF6356AD86.codesnippet`

```objc
(<#type#>)<#name#>
```

- `blarg` in `Block argument.codesnippet` and `EA231A0C-23B8-47CA-B6AF-D69367AA6C24.codesnippet`

```objc
(void (^)(<#argument#>))<#name#>
```

- `mmm` in `Method definition.codesnippet` and `08B6CA78-0C1E-4D6D-A9DD-0F560BAA5AA8.codesnippet`

```objc
- (<#id#>)<#method name#><##>;
```

- `doc` in `Method documentation.codesnippet` and `C67F9E35-A0E1-41F1-BE81-D81A52BB609B.codesnippet`

```objc
/**
 * <#description#>
 *
 * @param <#name#> <#description#>
 * @returns <#returns#>
 */
```

- `log` in `NSLog.codesnippet` and `9B303300-28CC-43BB-8115-B1A9F1F2EA45.codesnippet`

```objc
NSLog(@"<#message#>");
```

- `alert` in `UIAlertView.codesnippet` and `2562208A-CCF4-4210-91F1-451FC812D915.codesnippet`

```objc
UIAlertView *errorMessage = [[UIAlertView alloc] initWithTitle:@"<#title#>"
		                                               message:@"<#message#>"
		                                              delegate:<#delegate#>
                                             cancelButtonTitle:<#cancel button#>
                                             otherButtonTitles:<#other buttons#>];
[errorMessage show];
```

License
-------

Most of those snippets were taken from other repositories, all of which
had an MIT license. My own snippets also have an **MIT license**. The
license itself is in the LICENSE file.
