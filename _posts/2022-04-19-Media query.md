---
Layout:
Title:  "Media query"
Date:   "2022-04-19"
Categories:
---
# introduction
Media queries are a key part of responsive web design, as they allow you to create different layouts depending on the size of the viewport, but they can also be used to detect other things about the environment your site is running on, for example whether the user is using a touchscreen rather than a mouse.


# body
A media query is composed of an optional media type and any number of media feature expressions, which may optionally be combined in various ways using logical operators. Media queries are case-insensitive. Media types define the broad category of device for which the media query applies: all, print, screen. The type is optional (assumed to be all) except when using the not or only logical operators. A media query computes to true when the media type (if specified) matches the device on which a document is being displayed and all media feature expressions compute as true. Queries involving unknown media types are always false. Media types describe the general category of a given device. Although websites are commonly designed with screens in mind, you may want to create styles that target special devices such as printers or audio-based screenreaders. For example, this CSS targets printers: @media print { ... }
ou can also target multiple devices. For instance, this @media rule uses two media queries to target both screen and print devices: @media screen, print { ... }


# conclusion
Many media features are range features, which means they can be prefixed with "min-" or "max-" to express "minimum condition" or "maximum condition" constraints. For example, this CSS will apply styles only if your browser's viewport width is equal to or narrower than 12450px: @media (max-width: 12450px) { ... }