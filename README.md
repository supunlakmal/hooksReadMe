Okay, here is the updated main `README.md` file incorporating all the hooks found in the provided documentation files.

````markdown
# @supunlakmal/hooks

A collection of reusable React hooks designed to simplify common UI development tasks and abstract complex browser APIs.

## Installation

```bash
npm install @supunlakmal/hooks
# or
yarn add @supunlakmal/hooks
```
````

_(Note: Some hooks might have specific peer dependencies like `xlsx`. Check the individual hook documentation for details.)_

## Available Hooks

| Hook                                                                                                            | Description                                                                                                           |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| [useAnimation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useAnimation.md)                       | Manages a simple time-based animation loop using `requestAnimationFrame`.                                             |
| [useAsync](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useAsync.md)                               | Simplifies handling asynchronous operations (like API calls), managing loading, error, and success states.            |
| [useBreakpoint](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useBreakpoint.md)                     | Determines the currently active responsive breakpoint based on window width.                                          |
| [useBroadcastChannel](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useBroadcastChannel.md)         | Enables cross-tab/window communication using the Broadcast Channel API.                                               |
| [useCachedFetch](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useCachedFetch.md)                   | A `useFetch` variant with simple in-memory caching and TTL.                                                           |
| [useClickOutside](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useClickOutside.md)                 | Executes a callback when a click/touch event occurs outside of a specified DOM element.                               |
| [useClipboard](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useClipboard.md)                       | Provides functionality to interact with the system clipboard (copy/paste).                                            |
| [useContextMenu](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useContextMenu.md)                   | Provides state and logic for implementing a custom context menu (right-click menu).                                   |
| [useCopyToClipboard](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useCopyToClipboard.md)           | Provides a function to copy text to the clipboard and tracks status (uses fallback).                                  |
| [useCountdown](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useCountdown.md)                       | Manages a countdown timer with start, pause, and reset controls.                                                      |
| [useDarkMode](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDarkMode.md)                         | Manages application theme preference (dark/light mode) with OS detection and local storage persistence.               |
| [useDebounce](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDebounce.md)                         | Debounces a value, delaying updates until a certain time has passed without changes.                                  |
| [useDeepCompareEffect](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDeepCompareEffect.md)       | A `useEffect` variant that performs a deep comparison of dependencies.                                                |
| [useDerivedState](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDerivedState.md)                 | Computes derived state based on other values, recomputing only when dependencies change (wraps `useMemo`).            |
| [useDeviceMotion](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDeviceMotion.md)                 | Tracks device motion information (acceleration, rotation rate) via the `devicemotion` event.                          |
| [useDeviceOrientation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDeviceOrientation.md)       | Tracks the physical orientation of the device via the `deviceorientation` event.                                      |
| [useDrag](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDrag.md)                                 | Provides basic HTML Drag and Drop API event handling (`dragstart`, `drag`, `dragend`) for an element.                 |
| [useDraggable](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useDraggable.md)                       | Adds direct element draggability (positioning via transform) using pointer events, with bounds support.               |
| [useElementSize](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useElementSize.md)                   | Efficiently tracks the dimensions (width/height) of a DOM element using `ResizeObserver`.                             |
| [useErrorBoundary](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useErrorBoundary.md)               | Provides state management and control functions for React Error Boundaries.                                           |
| [useEventListener](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useEventListener.md)               | Robustly attaches event listeners to `window`, `document`, or elements, handling cleanup.                             |
| [useExportToExcel](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useExportToExcel.md)               | Exports data to Excel (.xlsx) files with automatic column sizing (requires `xlsx` library).                           |
| [useFiniteStateMachine](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useFiniteStateMachine.md)     | Manages complex component state using an explicit state machine definition.                                           |
| [useFetch](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useFetch.md)                               | A simple hook for fetching data, managing loading and error states.                                                   |
| [useFocusTrap](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useFocusTrap.md)                       | Traps keyboard focus within a specified container element when active (for modals, dialogs).                          |
| [useForm](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useForm.md)                                 | A basic hook for managing form state, input changes, and submission.                                                  |
| [useFormValidation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useFormValidation.md)             | A comprehensive hook for form state, validation (change/blur/submit), and submission handling.                        |
| [useFullscreen](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useFullscreen.md)                     | Enters and exits fullscreen mode for an element, tracking the current state.                                          |
| [useGeolocation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useGeolocation.md)                   | Tracks the user's geographic location using the Geolocation API.                                                      |
| [useHover](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useHover.md)                               | Tracks whether the mouse pointer is currently hovering over a specific DOM element.                                   |
| [useIdleTimer](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useIdleTimer.md)                       | Monitors user activity and triggers callbacks when the user becomes idle or active again.                             |
| [useInfiniteScroll](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useInfiniteScroll.md)             | Facilitates infinite scrolling using `IntersectionObserver` to trigger loading more data.                             |
| [useIntersectionObserver](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useIntersectionObserver.md) | Monitors the intersection of a target element with the viewport or an ancestor.                                       |
| [useInterval](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useInterval.md)                         | A declarative hook for setting intervals (`setInterval`) with automatic cleanup.                                      |
| [useIsFirstRender](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useIsFirstRender.md)               | Returns `true` if the component is rendering for the first time, `false` otherwise.                                   |
| [useIsMobile](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useIsMobile.md)                         | Detects if the current viewport is mobile-sized based on a configurable breakpoint.                                   |
| [useKeyCombo](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useKeyCombo.md)                         | Detects specific keyboard combinations (shortcuts) being pressed.                                                     |
| [useKeyPress](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useKeyPress.md)                         | Detects whether a specific key is currently being pressed down.                                                       |
| [useLocalStorage](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useLocalStorage.md)                 | Manages state persisted in `localStorage`, synchronizing across tabs.                                                 |
| [useLogger](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useLogger.md)                             | Development utility to log component lifecycle events and prop changes.                                               |
| [useLongPress](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useLongPress.md)                       | Detects long press gestures (mouse or touch) on a target element.                                                     |
| [useMap](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useMap.md)                                   | Manages state in the form of a JavaScript `Map`, providing immutable update actions.                                  |
| [useMediaQuery](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useMediaQuery.md)                     | Tracks the state of a CSS media query (e.g., viewport size, orientation, color scheme).                               |
| [useMergeRefs](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useMergeRefs.md)                       | Merges multiple React refs (callback or object refs) into a single callback ref.                                      |
| [useMount](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useMount.md)                               | Executes a callback function exactly once when the component mounts.                                                  |
| [useMutation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useMutation.md)                         | Simplifies handling asynchronous data modification operations (POST, PUT, DELETE), managing status.                   |
| [useNetworkSpeed](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useNetworkSpeed.md)                 | Provides information about the user's network connection (speed, type) using the Network Information API.             |
| [useOnlineStatus](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useOnlineStatus.md)                 | Tracks the browser's online/offline connection status.                                                                |
| [usePageVisibility](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/usePageVisibility.md)             | Tracks the visibility state of the current browser tab/page using the Page Visibility API.                            |
| [usePagination](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/usePagination.md)                     | Manages pagination logic for client-side data sets.                                                                   |
| [usePermission](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/usePermission.md)                     | Queries the status of browser permissions (geolocation, notifications, etc.) using the Permissions API.               |
| [usePortal](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/usePortal.md)                             | Simplifies the creation and management of React Portals.                                                              |
| [usePrevious](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/usePrevious.md)                         | Tracks the previous value of a state or prop from the last render.                                                    |
| [useQueryParam](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useQueryParam.md)                     | Synchronizes a React state variable with a URL query parameter.                                                       |
| [useReducerLogger](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useReducerLogger.md)               | Wraps `useReducer` to automatically log actions and state changes in development.                                     |
| [useRenderCount](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useRenderCount.md)                   | Tracks the number of times a component has rendered.                                                                  |
| [useResizeObserver](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useResizeObserver.md)             | Monitors changes to the dimensions of a target element using the `ResizeObserver` API.                                |
| [useRouteChange](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useRouteChange.md)                   | Executes a callback whenever the browser's URL path changes (handles `popstate` and `pushState`).                     |
| [useRovingTabIndex](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useRovingTabIndex.md)             | Implements the roving tabindex accessibility pattern for keyboard navigation within a group.                          |
| [useScrollPosition](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useScrollPosition.md)             | Tracks the current X and Y scroll position of the window or a specified element.                                      |
| [useScrollSpy](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useScrollSpy.md)                       | Monitors scroll position to determine which section element is currently active in the viewport.                      |
| [useScrollToTop](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useScrollToTop.md)                   | Provides a function to programmatically scroll the window to the top.                                                 |
| [useSessionStorage](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useSessionStorage.md)             | Manages state persisted in `sessionStorage` for the duration of the session.                                          |
| [useSet](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useSet.md)                                   | Manages state in the form of a JavaScript `Set`, providing immutable update actions.                                  |
| [useStateWithHistory](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useStateWithHistory.md)         | Manages state with undo/redo history tracking.                                                                        |
| [useStepper](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useStepper.md)                           | Manages state and navigation logic for multi-step processes (wizards, forms).                                         |
| [useSwipe](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useSwipe.md)                               | Detects swipe gestures (left, right, up, down) on touch-enabled devices for a specified element.                      |
| [useThrottle](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useThrottle.md)                         | Throttles a value, ensuring updates do not occur more frequently than a specified limit.                              |
| [useTimeout](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useTimeout.md)                           | A declarative hook for setting timeouts (`setTimeout`) with automatic cleanup.                                        |
| [useToggle](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useToggle.md)                             | Manages boolean state with convenient toggle, setOn, and setOff functions.                                            |
| [useTranslation](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useTranslation.md)                   | A basic hook for handling internationalization (i18n) with static resources.                                          |
| [useUnmount](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useUnmount.md)                           | Executes a cleanup function exactly once when the component unmounts.                                                 |
| [useUpdateEffect](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useUpdateEffect.md)                 | A `useEffect` variant that skips the effect execution after the initial render (mount).                               |
| [useVirtualList](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useVirtualList.md)                   | Performance optimization for rendering long lists by rendering only visible items (fixed height).                     |
| [useVisibility](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useVisibility.md)                     | Tracks whether a target element is currently visible within the viewport or an ancestor using `IntersectionObserver`. |
| [useWebSocket](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useWebSocket.md)                       | Manages WebSocket connections, state, messaging, and automatic reconnection.                                          |
| [useWindowSize](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useWindowSize.md)                     | Returns the current dimensions (width and height) of the browser window.                                              |
| [useWhyDidYouUpdate](https://github.com/supunlakmal/hooksReadMe/blob/main/docs/useWhyDidYouUpdate.md)           | Development utility to debug component re-renders by logging changed props.                                           |

## Usage

```jsx
import { useToggle, useDebounce } from "@supunlakmal/hooks";

function MyComponent() {
  // Use the hooks in your components
  const [isOpen, toggle] = useToggle(false);
  const debouncedValue = useDebounce(someValue, 500);

  return (
    <div>
      <button onClick={toggle}>{isOpen ? "Close" : "Open"}</button>
      <p>Debounced Value: {debouncedValue}</p>
    </div>
  );
}
```

## Features

- **TypeScript:** Written entirely in TypeScript with full type definitions.
- **Simplicity:** Designed with a straightforward and minimal API.
- **Reliability:** Focuses on abstracting browser APIs and common patterns correctly.
- **SSR Compatibility:** Hooks are generally designed to be safe in server-side rendering environments (where applicable).
- **Zero Dependencies:** Core hooks have no external runtime dependencies (unless noted).

## Contributing

Contributions, issues, and feature requests are welcome! Please feel free to submit a Pull Request or open an issue.

## License

This project is licensed under the ISC License - see the LICENSE file for details.

```

```
