# React Routing

## Review, Research, and Discussion

### Do child components have direct access to props/state from the parent?

Yes if the parent passes it down to the child as a prop.

### When a component “wraps” another component, how does the child component’s output get rendered?

By using props.children on the parent component.

### Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?

Yes this is possible, all components can be resusable.

### What trick can a parent use to share all props with it’s children

Parent will handle all state and functions then pass its states to the children who needs it.

## Vocab

- props.children - it is used to display whatever you include between the opening and closing tags when invoking a component.
- composition - the order or way you organize functions/components.
