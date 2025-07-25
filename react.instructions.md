---
applyTo: '**/*.tsx'
---

Coding standards, domain knowledge, and preferences that AI should follow.

# React Coding Standards and Preferences

<!-- Encourage to follow -->
## DO MORE

- Use functional components with hooks instead of class components.
- Use TypeScript for type safety.
- Use `useState` and `useEffect` hooks for state management and side effects.
- Use following snippet for functional components:
  ```tsx
  function MyComponent() => {
      return (
          <div>
              {/* Component JSX */}
          </div>
      );
  };

  export default MyComponent;
  ```

- Use `classnames` library for conditional class names. Search for `classnames` in the codebase to see how it's used.
- Use `useRef` for mutable references that do not trigger re-renders.
- Use `useContext` for global state management instead of Redux or MobX. Unless it was specified in the context to use Redux or MobX.
- Use callback for boolean state updates to avoid stale closures:
  ```tsx
  const [isOpen, setIsOpen] = useState(false);
  const toggleOpen = () => setIsOpen(prev => !prev);
  ```

- Limit the number of props passed to components. Maxed at 5. If a component has too many props, consider breaking it down into smaller components.
- Limit the number of `useState` hooks in a component. Maxed at 3. If a component has too many states, consider breaking it down into smaller components or hooks.
- Limit the number of `useEffect` hooks in a component. Maxed at 3. If a component has too many effects, consider breaking it down into smaller components or hooks.
- Limit the length of a comment. Maxed at 1. If a comment is too long, consider move it to the bottom of the file and use a `// NOTE:` prefix to indicate it's a note. This helps to keep the code clean and readable.


### MUST NOT DO

- Do not use `useEffect` for state initialization. Use `useState` directly.
- Do not use `useLayoutEffect` unless specified in the context.
- Do not use `useReducer` unless specified in the context.
- Do not use `useContext` for local state management. Use `useState` instead.
- Do not use `useRef` for state management. Use `useState` instead.
- Do not use `useImperativeHandle` unless specified in the context.
- Do not use `useDebugValue` unless specified in the context.
- Do not use inline functions in JSX. Define functions outside of the JSX return statement.
- Do not use inline styles. Use CSS modules or Tailwind CSS for styling.
- Do not use `any` type. Use specific types or interfaces.
- Do not use `console.log` for debugging. Use a proper logging library or debugging tools.
- Do not use `useMemo` and `useCallback` unless necessary specified in the context. They can lead to unnecessary complexity and performance issues if not used correctly.