# NgxGallery

A simple responsive native gallery component for Angular 19 based on kolkov/ngx-gallery.

## Features

- ✅ Angular 19 Support
- ✅ Responsive design
- ✅ Multiple image sizes support
- ✅ Thumbnail navigation
- ✅ Full-screen preview
- ✅ Touch/swipe support
- ✅ Keyboard navigation
- ✅ Customizable animations
- ✅ TypeScript support

## Installation

Install via [npm][npm] package manager:

```bash
npm install @murbanczyk-fp/ngx-gallery --save
```

## Quick Start

1. Import `NgxGalleryModule` in your module:

```typescript
import { NgxGalleryModule } from '@murbanczyk-fp/ngx-gallery';

@NgModule({
  imports: [NgxGalleryModule]
})
export class AppModule {}
```

2. Use the component in your template:

```html
<ngx-gallery [options]="galleryOptions" [images]="galleryImages"></ngx-gallery>
```

3. Configure in your component:

```typescript
import { NgxGalleryOptions, NgxGalleryImage } from '@murbanczyk-fp/ngx-gallery';

export class AppComponent {
  galleryOptions: NgxGalleryOptions[] = [
    {
      width: '600px',
      height: '400px',
      thumbnailsColumns: 4,
      imageAnimation: NgxGalleryAnimation.Slide
    }
  ];

  galleryImages: NgxGalleryImage[] = [
    {
      small: 'assets/1-small.jpg',
      medium: 'assets/1-medium.jpg',
      big: 'assets/1-big.jpg'
    },
    // ... more images
  ];
}
```

## Compatibility

- **Angular 19+**: Use version 19.x.x
- **Angular 18**: Use version 18.x.x
- **Angular 17**: Use version 17.x.x
- **Angular 16**: Use version 16.x.x
- **Angular 15**: Use version 15.x.x

## Development

### Building the Library

Run `ng build @murbanczyk-fp/ngx-gallery` to build the library. The build artifacts will be stored in the `dist/` directory.

### Running Tests

Run `ng test @murbanczyk-fp/ngx-gallery` to execute the unit tests via [Karma](https://karma-runner.github.io).

### Publishing

After building the library, run `npm run publish:lib` to publish to npm.

## Documentation

For detailed documentation and examples, visit the [base repository](https://github.com/kolkov/ngx-gallery) which contains comprehensive usage instructions.

## License

MIT License
