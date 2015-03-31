# TightConnect

*Note: TightConnect is currently in development. It is not yet released.*

## TightConnect Mission Statement

Using common, standard Web languages and proven cryptographic techniques, TightConnect aims to provide cryptographically secure selective data transmission between Webserver and client browser without undue impact on response time.

It accomplishes this through:

   * The use of standard JavaScript in the browser and PHP on the Webserver.

   * The use of Diffie-Hellman secure shared-key creation during intial session setup.

   * Secure user/server mutual authentication and user authorization based on a user password. This is accomplished by hashed challenge without transmission of the password, even in fixed hashed or encrypted form.

   * Fast encryption using a medium-strength algorithm (XXTEA) following session establishment, using a sequence of pseudo-unrelated keys to prevent attacks that require analysis of a large amount of encrypted data.

   * No need to slow down a Website by the use of SSL, which nonselectively encrypts entire pages, including large images, audio, video, and other content that may contain no secret information.

   * No need to incur the artificial and continuing expense of purchasing SSL trust certificates (which do not actually establish trust, since they can be purchased just as easily by malicious users who present forged identification as by honest and beneficent users).
 
## Demonstration Page

A working tutorial [demonstration and implementation](http://www.springtimesoftware.com/tightconnect/demo/) of the Diffie-Hellman algorithm for sharing a secret keyword has been created. It includes a detailed description and references.

## Limitations of TightConnect

   * TightConnect is currently in development. It is not yet released.

   * Requires JavaScript be enabled in browser.

   * Meant for use with recent browsers only; may cause a timeout error with very old browsers and will not work with text-only browsers.

   * Current version, like other similar solutions, is vulnerable to a "Man In The Middle" (MITM) attack, because the entity in the middle of the communications channel can modify the downloaded JavaScript code.

## Acknowledgments

   * Thanks to [Dr. Leemon Baird](http://www.leemon.com) for use of his public domain **BigInt.js Big Integer Library**.

   * Thanks to [Makoto Matsumoto and Takuji Nishimura](http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt.html) of the Department of Mathematics of Hiroshima University (Japan) for use of their *Mersenne Twister* function (see TightConnect source distribution for copyright notice).

   * Thanks to [Brian Turek](http://caligatio.users.sourceforge.net) for use of the SHA-256, SHA-512, and HMAC functions from his `jsSHA` library.

*Note: This project was automatically exported from `code.google.com/p/tightconnect`.*
