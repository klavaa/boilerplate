# Klavaa

Klavaa is a small set of utility classes for HTML email development.

## Sections

The boilerplate have at the beginning base styles, which apply some resets to the email clients and browsers. And the rest of the css are utilities mostly for mobile development.

## Usage

Remove links on _addresses_ and _phone numbers_ by adding the class `.mobile-link` to a `td` and a `span`.

```html
<tr>
	<td align="center" class="mobile-link" style="font-family: Arial, Tahoma, sans-serif; font-size: 14px; line-height: 16px; font-weight: normal; color: #000000;">
		<span class="mobile-link">P sherman wallaby 42, Sidney</span>
	</td>
</tr>
```

Hide and show elements on mobile with `hide-m` and `show-for-small`. The tables can't be hidden on some email clients.

```html
<tr>
	<td align="center" style="">
		<img class="hide-m" src="desktop-image.png" width="600" height="400" alt="My awesome image" style="display:block; border: none; max-width:600px;" />
		<span class="show-for-small" style="display:none; max-height:0px; overflow:hidden; width:0px; line-height:0px;">
			<img src="mobile-image.png" width="300" height="400" alt="My awesome mobile image" style="display:block; border: none; max-width:300px;" />
		</span>
	</td>
</tr>
```

Responsive resize and center images on mobile with `resize-image` and `center-image`.

```html
<img class="resize-image center-image" src="image.png" width="300" height="50" alt="My awesome image" style="display:block; border: none; max-width:300px;" />
```

Change the width of elements (mostly tables) on mobile with `w100`, `w90` and `w50`.

```html
<table class="w100" border="0" cellpadding="0" cellspacing="0" width="600" align="center" style="width: 600px;">
	<tbody>
		<tr>
			<td align="center" style="">
				My content.
			</td>
		</tr>
	</tbody>
</table>
```

The rest of the utility classes are self explanatory, most of them are for changing text size on mobile and adjust paddings.

| Class        | Description           |
| ------------- | ------------- |
| mobile-link     | Removes the anchor styling that some email clients add. |
| hide-m      | Hide an element on mobile.      |
| show-for-small | Show an element on mobile.      |
| no-float | Remove floats for an element on mobile.  |
| block | Change the display to block for an element on mobile.   |
| resize-image | Add responsiveness to the images on mobile.  |
| center-image | Center an image on mobile.   |
| text-center | Center the text on mobile.   |
| font-14 | Change the font to 14px on mobile.   |
| font-16 | Change the font to 16px on mobile.   |
| font-18 | Change the font to 18px on mobile.   |
| font-20 | Change the font to 20px on mobile.   |
| font-22 | Change the font to 22px on mobile.   |
| pad-t-0 | Remove the padding top on mobile.   |
| pad-r-0 | Remove the padding right on mobile.   |
| pad-b-0 | Remove the padding bottom on mobile.   |
| pad-l-0 | Remove the padding left on mobile.   |
| pad-t-20 | Add 20px of padding to the top on mobile.   |
| pad-r-20 | Add 20px of padding to the right on mobile.   |
| pad-b-20 | Add 20px of padding to the bottom on mobile.   |
| pad-l-20 | Add 20px of padding to the left on mobile.   |
| pad-0 | Remove all padding of an element on mobile.   |
| pad-10 | Add 10px of padding on all directions.   |
| pad-20 | Add 20px of padding on all directions.   |
| pad-sides-0 | Remove padding on the right and left on mobile.   |
| pad-sides-10 | Add 10px of padding to the right and left on mobile.   |
| pad-sides-20 | Add 20px of padding to the right and left on mobile.   |
| w100 | Change the width to 100% on mobile.   |
| w90 | Change the width to 90% on mobile.   |
| w50 | Change the width to 50% on mobile.   |

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](./LICENSE.md)
