# tailwind CSS

## Why Tailwind?
Tailwind is a **design system** that replaces custom styling and CSS with a global theme which consists of utility classes. 

It's more flexible and often results in better looking designs than its predesessors like Material Design/UI and Bootstrap.

You can create great looking designs without adding any custom styles to individual components.


## Tradeoffs
**Missing components**. MUI is faster to use out of the box. Tailwind does not have UI components for everything that MUI does. But it does have a large component library (500+ components).

**New maintainability issue**: "The biggest maintainability concern when using a utility-first approach is managing commonly repeated utility combinations."

## Getting Started

### Download Files
Many of Tailwind's resources require a license. Files can be downloaded from [tailwindcss.com](https://tailwindcss.com).

### VS Code Extension
There is a tailwindcss extension for VS Code.

### prettier plugin
There is a tailwindcss prettier plugin, too.

### Catalyst UI Kit
1. Download the files
2. Copy components
3. I prefer React components to be named in CamelCase so I renamed the files and their inter-depencencies (imports).

## Example
See [here](https://tailwindcss.com/docs/utility-first). Tailwind uses CSS utility classes to style components:

```html
<div class="p-6 max-w-sm mx-auto bg-white rounded-xl shadow-lg flex items-center space-x-4">
  <div class="shrink-0">
    <img class="h-12 w-12" src="/img/logo.svg" alt="ChitChat Logo">
  </div>
  <div>
    <div class="text-xl font-medium text-black">ChitChat</div>
    <p class="text-slate-500">You have a new message!</p>
  </div>
</div>
```

This uses:
- Tailwind’s flexbox utilities: `flex` `shrink`
- Padding: `p-6`
- Width and height: `max-w-sm`, `w-12`, `h-12`
- Margin: `mx-auto`
- Background color: `bg-white`
- Border Radius: `rounded-xl`
- Box shadow: `shadow-lg`
- Space between: `space-x-4`
- Typography: `text-xl`, `text-black`, `font-medium`

🎉 This styles the component without writing a single line of custom CSS!!!

```html
<div class="py-8 px-8 max-w-sm mx-auto bg-white rounded-xl shadow-lg space-y-2 sm:py-4 sm:flex sm:items-center sm:space-y-0 sm:space-x-6">
  <img class="block mx-auto h-24 rounded-full sm:mx-0 sm:shrink-0" src="/img/erin-lindford.jpg" alt="Woman's Face" />
  <div class="text-center space-y-2 sm:text-left">
    <div class="space-y-0.5">
      <p class="text-lg text-black font-semibold">
        Erin Lindford
      </p>
      <p class="text-slate-500 font-medium">
        Product Engineer
      </p>
    </div>
    <button class="px-4 py-1 text-sm text-purple-600 font-semibold rounded-full border border-purple-200 hover:text-white hover:bg-purple-600 hover:border-transparent focus:outline-none focus:ring-2 focus:ring-purple-600 focus:ring-offset-2">Message</button>
  </div>
</div>
```

This uses:
- Spacing: `px-4`, `px-y`, `space-y-2`
- Hover: `hover:border-transparent`, `hover:bg-purple-600`, `hover:text-white`  
- Focus: `focus:outline-none`, `focus:ring-2`, `focus:ring-purple-600`, `focus:ring-offset-2`
- Border classes: `border` `border-purple-200` `border-transparent` `border-`
- Text align: `text-center`
- Responsive: `sm:py-4`, `sm:flex`

## Core classes

### Flexbox, Padding, Spacing
- Flex: `flex space-x-4`, `flex-1`, `flex-auto`
- Justify-content: `justify-center` (start, end, between, evenly, ...)
- Align items: `items-center` (start, end, ...)
- ⁉️ Grid: `grid`
- Padding: `p-*`, `px-*`, `py-*`, `pr-*`, `pt-*`, `pl-*`, `pb-*`
- Margin: `m-*`, `mx-*`, `my-*`, `mr-*`, `mt-*`, `ml-*`, `mb-*`
- Space: `space-x-*`, `space-y-*`
- Container: `container` (fixes a max width)
- Wrap
- Basis (size of items)
- Grow (allow item to fill space)

### Typography
- Font Size: `text-xs`, `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-*xl` (*=2-9)
- Font Weight: `font-medium` (`thin`, `extralight`, `light`, `normal`, `medium`, `semibold`, `bold`, `extrabold`, `black`)
- Line height: `leading-normal`, `leading-tight`, `leading-snug`, `leading-relaxed`, `leading-loose`
- Alignment: `text-left`, `text-center`, `text-right`...
- Color: `text-*`
- Overflow
- Transform

### Responsive Designs

### Borders, shadow, dividers
- Borders: `border`, `border-width-*`, `border-color-*`
- Box shadow: `shadow`, `shadow-md`, ...
- Dividers: `divide-y`, `divide-x`, `divide-color`
- Rings & outlines: also configurable!

### Background
- `bg-*`
- bg attachment: `bg-fixed`, `bg-local`, `bg-scroll`
- Images: Add to theme or use `bg-[url('/img/hero-pattern.svg')]`
- Gradient: `h-14 bg-gradient-to-r from-cyan-500 to-blue-500`
  
### States (hover, focus, etc.)
[See here](https://tailwindcss.com/docs/hover-focus-and-other-states)

### Layouts
- Overflow
- Display: `hidden`, `flex`, `inline`, `grid`
- 

### Visual effects & Animations
- Photo Filters: [Blur](https://tailwindcss.com/docs/blur), Grayscale, etc
- Aspect ratios
- Animations: `animate-spin`, `animate-ping`, `animate-pulse`, `animate-bounce`

### Misc
- Scroll classes
- Cursors

