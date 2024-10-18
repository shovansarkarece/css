# Font Properties
![image](https://github.com/user-attachments/assets/bad0b915-d02d-444b-9f32-feb9cc374f33)

### Font Family:- The `font-family` property allows you to specify the font used for text.

### Font Size:- The `font-size` property controls the size of text.
- **You can use various units like pixels (`px`), ems (`em`), percentages (%), or keywords (e.g., `small`, `medium`, `large`) to set the size.**
### Font Weight:- The `font-weight` property defines the thickness of text characters, ranging from `100` (thin) to `900` (bold).
### Font Style:- The `font-style` property allows you to apply styles like italic to text.
- **Common values include `normal` (default), `italic`, and `oblique`.**
### Font Variant:- The `font-variant` property is used to control the appearance of text characters by modifying their variant forms.
- **value: normal, small-caps**
### Import Font
```
@import url("https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;500;600;700;800;900&display=swap");

@font-face {
  font-family: "thapaFont";
  src: url("./font/Fortune.otf") format("OpenType");
}
```
### Common font formats and their corresponding format values are:

- **TrueType Font (.ttf): format('truetype') or format('opentype')**
- **WOFF Font (.woff): format('woff')**
- **WOFF2 Font (.woff2): format('woff2')**
- **Embedded OpenType Font (.eot): format('embedded-opentype')**
- **SVG Font (.svg): format('svg')**
