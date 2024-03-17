# ngx-navigate-back

ngx-navigate-back is a lightweight Angular library designed to simplify navigation management within Angular applications. With ngx-navigate-back, you can easily implement a "back" functionality similar to the browser's native back button, allowing users to navigate to the previous page within your Angular application.

## Features

- **Simple Integration**: Easy to integrate into your Angular application.
- **Record Navigation History**: Record the navigation history to enable smooth backward navigation.
- **Retrieve Navigation History**: Get the navigation history as an array.
- **Navigate Back**: Go back to the previous page with a simple function call.

## Functions
- recordUrlHistory(): Begins recording the navigation history.
- getHistory(): Retrieves the navigation history as an array.
- navigateBack(): Navigates back to the previous page.

## Installation

Install ngx-navigate-back via npm:

```bash
npm install ngx-navigate-back
```

## Usage

1. Import `NgxNavigateBackService` in your Angular component:

```typescript
import { NgxNavigateBackService } from 'ngx-navigate-back';
```

2. Inject `NgxNavigateBackService` into your component:

```typescript
constructor(public navigation: NgxNavigateBackService) {
  this.navigation.recordUrlHistory();
}
```

3. Use the `navigateBack()` function to implement the "back" functionality:

```html
<button (click)="navigation.navigateBack()">Back to Previous Page</button>
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
