# TP2 answers

## Question 1
TypeScript complains because the old `Item` values do not include the newly required `claimed` field.

## Question 2
The counter shows total reports and reports still waiting. The footer shows `Platform.OS`; the word comes from React Native's platform detection.

## Question 3
Both screens use the shared `items` state from `ItemsContext`, provided above the navigator.

## Question 4
The screen uses `useLocalSearchParams` to read the `id` route parameter.

## Question 5
The claimed card becomes faded and shows `✓ Claimed`; the waiting count decreases. iPhone renders its native iOS switch control.

## Question 6
`/item/999` shows the not-found message. No confirmation dialog appears because the remove action is not rendered.

## Question 8: navigation map
```text
Home (/) --Report an item--> Add (/add) --Save/router.back--> Home
Home (/) --tap card--> Item (/item/:id)
Item --switch--> toggleClaimed; --remove/confirm--> removeItem/router.back--> Home
All screens receive shared data from ItemsProvider in _layout.tsx.
```
