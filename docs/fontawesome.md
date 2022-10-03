# Fontawesome

This Boilerplate application comes with `Fontawesome 6 Free` pre-installed.

## Example

Below is a basic example of how to use Fontawesome in this application

Add this to your HTML file

```html
<fa-icon [icon]="faFire" class="text-orange-500"></fa-icon>
```

In your component you need to import your desired icons like the following:

```typescript
import { faFire } from '@fortawesome/free-solid-svg-icons';
```

Then declare a new variable for each icon:

```typescript
faFire = faFire;
```