# WG21 SG16 Unicode study group
SG16 is an ISO/IEC JTC1/SC22/WG21 C++ study group tasked with improving Unicode and text processing support within the C++ standard.

If you would like to contribute to the discussion, please join us on [<img src="http://slack.com/favicon.ico" height="16"/>Slack](https://cpplang.slack.com/messages/sg16_unicode) at https://cpplang.slack.com/messages/sg16_unicode
(an invitation can be requested at https://cpplang.now.sh) and subcribe to our mailing list at
https://lists.isocpp.org/mailman/listinfo.cgi/sg16.

Meetings are generally held twice a month; invitations are sent to the mailing list.  Summaries of past meetings are available at https://github.com/sg16-unicode/sg16-meetings/blob/master/README.md.

A standing paper that describes our intended scope, directives, guidelines and constraints is available at [P1238 - SG16: Unicode Direction][P1238].  Anyone wanting to follow or contribute to SG16 should become familiar with it.

The following sections list papers and projects currently under our purview.  Additionally, we provide input to proposals that originate elsewhere within WG21 when those proposals touch on topics listed in [P1253 - Guidelines for when a WG21 proposal should be reviewed by SG16][P1253].

# WG21 (C++) Papers

## Active Papers and Projects

WG Number     | Title/Notes/Links
------------- | -----
\<None\>      | Boost.Text: What a c++ standard Unicode library might look like<br/>[Code repository](https://github.com/tzlaine/text)<br/>[Documentation](https://tzlaine.github.io/text/doc/html/index.html)
[P2246][]     | Character encoding of diagnostic text
[P2201][]     | Mixed string literal concatenation
[P2194][]     | The character set of C++ source code is Unicode
[P2178][]     | Misc lexing and string handling improvements
[P2071][]     | Named universal character escapes
[P2020][]     | Locales, Encodings and Unicode
[P1953][]     | Unicode Identifiers And Reflection
[P1949][]     | C++ Identifier Syntax using Unicode Standard Annex 31
[P1885][]     | Naming Text Encodings to Demystify Them
[P1859][]     | Standard terminology for execution character set encodings
[P1629][]     | Standard Text Encoding
[P1628][]     | Unicode character properties
[P0244][]     | Text\_view: A C++ concepts and range based character encoding and code point enumeration library

## Accepted Papers

The following papers have been adopted for an ISO standard.

WG Number     | Standard    | Title/Notes/Links
------------- | --------    | -----
[P2029][]     | C++23       | Proposed resolution for core issues 411, 1656, and 2333; numeric and universal character escapes in character and string literals
[P1892][]     | C++20       | Extended locale-specific presentation specifiers for std::format
[P1868][]     | C++20       | 🦄 width: clarifying units of width and precision in std::format
[P1423][]     | C++20       | char8\_t backward compatibility remediation
[P1139][]     | C++20       | Address wording issues related to ISO 10646
[P1041][]     | C++20       | Make char16\_t/char32\_t string literals be UTF-16/32
[P1025][]     | C++20       | Update The Reference To The Unicode Standard
[P0645][]     | C++20       | Text Formatting
[P0482][]     | C++20       | char8\_t: A type for UTF-8 characters and strings

## Inactive Papers

The following papers are no longer being pursued.

WG Number     | Title/Notes/Links
------------- | -----
~~[P1880][]~~ | ~~uNstring Arguments Shall Be UTF-N Encoded~~<br/>(This proposal was withdrawn by the author upon determining that the complexity of the required wording updates would outweigh their benefits)
~~[P1879][]~~ | ~~Please Don't Rewrite My String Literals~~<br/>(This proposal was withdrawn by the author)
~~[P1854][]~~ | ~~Conversion to execution encoding should not lead to loss of meaning~~<br/>(The author incorporated this proposal in to [P2178][])
~~[P1844][]~~ | ~~Enhancement of regex~~<br/>(Severe ABI concerns prevent updating `std::regex`.  We will explore deprecating and replacing it)
~~[P1097][]~~ | ~~Named character escapes~~<br/>(Superceded by P2071)
~~[P0353][]~~ | ~~Unicode Friendly Encoding Conversions for the Standard Library~~<br/>(This proposal is not being advocated at this time; more foundational concerns need to be addressed first)
~~[P0169][]~~ | ~~regex with Unicode character types~~<br/>(This proposal is not being advocated at this time; more foundational concerns need to be addressed first)

# WG14 (C) Papers

## Active Papers

WG Number     | Status      | Title/Notes/Links
------------- | ------      | -----
[N2595][]     |             | Restartable and Non-Restartable Functions for Efficient Character Conversions | r4<br/>(Previously [N2431][N2431 (R0)], [N2440][N2440 (R1)], and [N2500][N2500 (R2)])
[N2594][]     |             | Mixed Wide String Literal Concatenation
[N2231][]     |             | char8\_t: A type for UTF-8 characters and strings

## Inactive Papers

WG Number     | Title/Notes/Links
------------- | -----
~~[N2431][]~~ | ~~Restartable and Non-Restartable Functions for Efficient Character Conversions~~<br/>(Superceded by [N2440][])
~~[N2440][]~~ | ~~Restartable and Non-Restartable Functions for Efficient Character Conversions | r1~~<br/>(Superceded by [N2500][])
~~[N2500][]~~ | ~~Restartable and Non-Restartable Functions for Efficient Character Conversions | r2~~<br/>(Superceded by [N2595][])

[N2595]: http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2595.pdf
[N2594]: http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2594.htm
[N2500]: http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2500.pdf
[N2431]: http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2431.pdf
[N2231]: http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2231.htm
[P2246]: https://wg21.link/p2246
[P2201]: https://wg21.link/p2201
[P2194]: https://wg21.link/p2194
[P2178]: https://wg21.link/p2178
[P2071]: https://wg21.link/p2071
[P2029]: https://wg21.link/p2029
[P2020]: https://wg21.link/p2020
[P1953]: https://wg21.link/p1953
[P1949]: https://wg21.link/p1949
[P1892]: https://wg21.link/p1892
[P1885]: https://wg21.link/p1885
[P1880]: https://wg21.link/p1880
[P1879]: https://wg21.link/p1879
[P1868]: https://wg21.link/p1868
[P1859]: https://wg21.link/p1859
[P1854]: https://wg21.link/p1854
[P1844]: https://wg21.link/p1844
[P1629]: https://wg21.link/p1629
[P1628]: https://wg21.link/p1628
[P1423]: https://wg21.link/p1423
[P1253]: https://wg21.link/p1253
[P1238]: https://wg21.link/p1238
[P1139]: https://wg21.link/p1139
[P1097]: https://wg21.link/p1097
[P1041]: https://wg21.link/p1041
[P1025]: https://wg21.link/p1025
[P0645]: https://wg21.link/p0645
[P0482]: https://wg21.link/p0482
[P0244]: https://wg21.link/p0244
[P0353]: https://wg21.link/p0353
[P0169]: https://wg21.link/p0169
