# CardFooter

CardFooter renders an optional footer within a [`<Card />`](../card/README.md).

## Usage

```jsx
import { Card, CardFooter } from '@wordpress/components';

const Example = () => (
	<Card>
		<CardFooter>...</CardFooter>
	</Card>
);
```

### Flex

Underneath, CardFooter uses the layout component [`<Flex/>`](../../flex/flex/README.md). This improves the alignment of child items within the component.

```jsx
import {
	Button,
	Card,
	CardFooter,
	FlexItem,
	FlexBlock,
} from '@wordpress/components';

const Example = () => (
	<Card>
		<CardFooter>
			<FlexBlock>Content</FlexBlock>
			<FlexItem>
				<Button>Action</Button>
			</FlexItem>
		</CardFooter>
	</Card>
);
```

Check out [the documentation](../../flex/flex/README.md) on `<Flex/>` for more details on layout composition.

## Props

### isBorderless

Determines the border style of the card.

-   Type: `Boolean`
-   Required: No
-   Default: `false`

### isElevated

Determines the elevation style of the card.

-   Type: `Boolean`
-   Required: No
-   Default: `false`

### isShady

Renders with a light gray background color.

-   Type: `Boolean`
-   Required: No
-   Default: `false`

### size

Determines the amount of padding within the component.

-   Type: `String`
-   Required: No
-   Default: `medium`

Note: This component is connected to [`<Card />`'s Context](../card/README.md#context). Passing props directly to this component will override the props derived from context.
