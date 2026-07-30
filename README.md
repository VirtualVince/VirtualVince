# Vincente Sequeira

I build software that runs machines, and the infrastructure that keeps it running.

That covers more ground than it sounds like. It is the reason a Linux VPS I administer
and an Arduino on my bench are the same interest rather than two hobbies: both are about
understanding the layer underneath, the one everything else depends on and nobody looks
at until it breaks. I run a freelance practice under **Virtual Vince**, and I am
building toward embedded and systems work.

I am not a frontend developer. I ship frontends when a client needs one, and I would
rather be under the surface.

---

## Orpheus

Version control for music production. Git works badly on DAW projects because they are
large binary files with no stable identity inside them, so a one-note change looks like
a whole-file rewrite. Orpheus makes those projects genuinely diffable.

I am a co-founder. My work is on the backend: the Convex schema, the track mutations,
and the input validation that guards what reaches the database. I also contributed to
the DAW diffing design and to the architecture of `flparse`, our Rust crate that parses
FL Studio's binary event stream and re-encodes it byte-for-byte.

The interesting problem is identity. FL Studio's format has no GUIDs anywhere, so
channels, patterns and mixer inserts are identified purely by position. Work out that a
user reordered two channels rather than deleted and recreated them, and you get a
readable diff. Get it wrong and every save looks like a rewrite. Ableton is the
opposite case, with stable persistent IDs but heavy save noise to filter out. Every
prior attempt at this either handled one DAW or drowned in false positives.

TypeScript · Rust · Convex · Bun · Turborepo · Nix. Private repo, four contributors.

## Elizabeth Gardens Creative Collective

A community arts organization, running on a VPS I provisioned and administer end to
end. Bare Ubuntu Server upward: HestiaCP, user accounts, DNS, firewall, and my own
backup routine. It is multi-tenant, hosting other artists alongside the main site.

The build itself is roughly 5,700 lines of PHP across eleven plugins, and the approach
matters more than the volume. Rather than clicking through the WordPress admin, I wrote
idempotent provisioning plugins that create the pages, navigation, Elementor layouts,
forms and content programmatically, each behind a preview-and-confirm step. Site
structure lives in version control as data, not as a sequence of remembered UI actions.

The one built to stay is an activity log: its own database table created on activation,
a schema version key for migrations, configurable account exclusions, and capture of
exact diffs for every content edit alongside plugin and publishing events. The board can
see who changed what, which is what a volunteer-run organization actually needs.

Ubuntu · HestiaCP · PHP · WordPress · MySQL · [creativecollectiveonline.com](https://creativecollectiveonline.com/)

## ChironAI

The AI arm of my practice: training teams to use AI properly, plus agent setup and
automation for small businesses. Most of the work is unglamorous, which is the point.
Businesses do not need a model, they need the boring integration around it to be
reliable.

[chiron.virtualvince.ca](https://chiron.virtualvince.ca/)

## Client work

- **[Radiant Roots Vitality](https://www.radiantrootsvitality.com/)**: health practice.
  Next.js, TypeScript, Tailwind, with Google Maps and a Fullscript storefront handoff.
  Ongoing hosting and maintenance retainer.
- **[My YAYBI Way](https://myyaybiway.me/)**: Next.js, TypeScript, Tailwind, pulling
  live products, images and metadata from a Shopify storefront into a custom front end
  rather than theming Shopify itself.
- **[K2E Canada](https://www.k2e.ca/)**: professional education. Shopify storefront
  with custom Liquid.

## Bench work

**[r3builds](https://github.com/VirtualVince/R3Builds)** is ten Arduino Uno builds
ordered so each earns one transferable skill the next one leans on: GPIO and timing,
debounce, PWM, UART, ADC, I2C, SPI, a sensor-to-actuator control loop, a finite state
machine, and IR protocol decode into actuation. It is deliberately unglamorous
groundwork. The point is reading a datasheet and speaking a protocol without a library
holding my hand.

It feeds a longer roadmap: PID and IMU sensor fusion, RF and SDR work toward a
receive-only satellite ground station, embedded Linux, and portable power. I am filming
the whole thing, failures included.

## Other work

- **[cifar10-regularization-study](https://github.com/VirtualVince/cifar10-regularization-study)**:
  a controlled four-model comparison isolating what dropout, L2 and augmentation each
  contribute. Starts from a deliberately overparameterized 12M-parameter dense network
  and fixes it one technique at a time.
- **[employee-management-system](https://github.com/VirtualVince/employee-management-system)**:
  Apollo GraphQL API over MongoDB with JWT auth and Cloudinary uploads, plus a
  route-guarded Angular client.
- **[ios-product-catalog](https://github.com/VirtualVince/ios-product-catalog)**: Swift
  and UIKit, on a Core Data stack whose managed object model is built in code rather
  than from a `.xcdatamodeld` bundle, so schema changes are reviewable in a diff.

## Tools

Go, TypeScript, Python, C++, C#, Java, PHP, Lua, SQL, Liquid. Linux and Ubuntu Server,
HestiaCP, DNS and firewall administration. Node, Express, Next.js, React, Angular,
ASP.NET. PostgreSQL, MongoDB, MySQL, SQLite, Convex. AWS, Azure, GCP, Vercel. Arduino,
C for microcontrollers. Arch, fish, Neovim, Git.

## Elsewhere

Practice and client work at **[virtualvince.ca](https://virtualvince.ca)** ·
[LinkedIn](https://www.linkedin.com/in/vincente-sequeira-1824b4245/) ·
[YouTube](https://www.youtube.com/@virtualvincebuilds)
