# UI Testing Notes

### `<Popover>` vs `<Dropdown>`

When simulating clicks on these components, do the following:

```js
// for Popovers
import userEvent from '@testing-library/user-event'
await userEvent.click('Hello world')

// for Dropdowns
import clickDropdown from 'tests/helpers'
clickDropdown('Hello world')
```

### Rules

- All tests should be run consistently (avoid situations whereby tests fails "sometimes")
