[![npm](https://img.shields.io/npm/v/@zibuthe7j11/nulla-numquam-quos.svg)](https://www.npmjs.com/package/@zibuthe7j11/nulla-numquam-quos) ![downloads](https://img.shields.io/npm/dt/@zibuthe7j11/nulla-numquam-quos.svg) [![CI](https://github.com/zibuthe7j11/nulla-numquam-quos/actions/workflows/ci.yml/badge.svg)](https://github.com/zibuthe7j11/nulla-numquam-quos/actions)

# Make-Event-Props

A function that, given props, returns an object of event callback props optionally curried with additional arguments.

This package allows you to pass event callback props to a rendered DOM element without the risk of applying any invalid props that could cause unwanted side effects.

## tl;dr

- Install by executing `npm install @zibuthe7j11/nulla-numquam-quos` or `yarn add @zibuthe7j11/nulla-numquam-quos`.
- Import by adding `import makeEventProps from '@zibuthe7j11/nulla-numquam-quos'`.
- Create your event props object:
  ```ts
  const eventProps = useMemo(
    () => makeEventProps(props, (eventName) => additionalArgs),
    [additionalArgs],
  );
  ```
- Use your event props:
  ```tsx
  return <div {...eventProps} />;
  ```

## License

The MIT License.

## Author

<table>
  <tr>
    <td >
      <img src="https://avatars.githubusercontent.com/u/5426427?v=4&s=128" width="64" height="64" alt="Wojciech Maj">
    </td>
    <td>
      <a href="https://github.com/wojtekmaj">Wojciech Maj</a>
    </td>
  </tr>
</table>
