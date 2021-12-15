# react-scroll-to-top-component
react-scroll-to-top-component

```
import { useLayoutEffect } from "react";
import { useLocation } from "react-router-dom";

export default function ScrollToTop() {
  const { pathname } = useLocation();

  useLayoutEffect(() => {
    window.scrollTo(0, 0);
  }, [pathname]);

  return null;
}
```

## HOW TO USE
Call the component on you layout,page or router, like this:

```
function Index() {
  return (
    <Router>
      <ScrollToTop />
      <App />
    </Router>
  );
}
```
