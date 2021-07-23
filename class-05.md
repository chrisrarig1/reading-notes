# CSS: Images, Color, and Text

## Images

### Adding An Image

- Adding images to your page requires the use of a `<img>` tag. Inside the tags we use `src="filename.jpg"` this grabs the photo from its file location. You can also add content to your picture by adding a description `alt="description"` or a title `title="title"`. Here is a full code example:

    `<img src="filename.jpg" alt="this is a picture of" title="title of picture" />`

### Formatting An Image

- When adjusting the size of a picture you can use **height** and **width**. These are measured in pixels. Example:

    `<img src="filename.jpg" alt="this is a picture of" title="title of picture" width="450" height="500" />`

- After sizing the picture it is important to orient the image correctly on the page. You can place it before a paragraph, at the start of the paragraph or in a paragraph. If you place it within the paragraph the text will be separated and is not appealing.
- Images are usually saved as **JPEGs** and anything that uses flat colors should be saved as a **GIF**.

## Color

- Using color on your website not only gives it a appealing appearance, but can also cause intrigue to the viewer.

- CSS uses three color identifiers. **RGB Values**, **HEX Codes**, and **Color Names**.
  - **RGB**: These are values for Red, Green, and Blue and show in code as this `rgb(95,185,200)`
  - **HEX**: This is a hexadecimal code for Red, Green, and Blue.
        `#66cdaa`
  - **Color Names**: Straight names of colors.
        `red`
- CSS also added a fourth value where you can change the opacity of the color. It is labeled with an `a` in `rgba`.

## Text

- CSS allows you to change and updated the format of your text giving some flare rather than having the boring old default text.

### Font Style/Size

- `font-family=` This will give you a select amount of font styles to choose from. Typically you want to be consist on this
- `font-size=` This gives you the ability to adjust the size of your font.

### Transform Fonts

- `font-weight: bold or normal;` This causes the font to be bold or normal.
- `font-style: italic or normal or oblique;` This causes the font to be italic, normal or appear oblique.
- `text-transform:` this allows you to change the font to uppercase, lowercase, or capitalize the font.
- `text-decoration:` this allows you to underline, over-line, line-through, or blink the text

### Alignment

- `text-align` Assigns alignment to the left, right, center, or justify the text
- `vertical-align` This allows you to align text with images.
- `text-indent:` This will indent the first part of the paragraph of text

# Useful Links

- [CSS Text](https://www.w3schools.com/css/css_text.asp)
- [CSS Color](https://www.w3schools.com/css/css_colors.asp)
- [CSS](https://www.w3schools.com/css/default.asp)

# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley,2011.
