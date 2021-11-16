# sticky

Sticky is a lightweight alternative to `position: sticky` polyfills

# install

```
npm i @silen/sticky
```

# usage

```ts
import Sticky from '@silen/sticky';

const selector: string | Element = '.child';
const option: {
  customStickyChangeNumber?: number | null;
  noStyles?: boolean;
  stickyBitStickyOffset?: number;
  parentClass?: string;
  scrollContainer?: Element | string | Window;
  stickyClass?: string;
  stuckClass?: string;
  stickyChangeClass?: string;
  useStickyClasses?: boolean;
  useFixed?: boolean;
  useGetBoundingClientRect?: boolean;
  verticalPosition?: 'top' | 'bottom';
  applyStyle?: Function;
} = { scrollContainer: document.querySelector('.container') };

const sticky = new Sticky(selector, option);
```
