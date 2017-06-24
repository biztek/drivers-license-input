[![Build Status](https://travis-ci.org/biztek/drivers-license-input.svg?branch=master)](https://travis-ci.org/biztek/drivers-license-input)

[![Sauce Test Status](https://saucelabs.com/buildstatus/biztek)](https://saucelabs.com/u/biztek)

[![Sauce Test Status](https://saucelabs.com/browser-matrix/biztek.svg)](https://saucelabs.com/u/biztek)

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/biztek/drivers-license-input)

_[Demo and API Docs](https://biztek.github.io/drivers-license-input/components/drivers-license-input/)_

# \<drivers-license-input\>

`<drivers-license-input>` is a Input field that validates the driver license based on the Json file.

```html
<drivers-license-input></drivers-license-input>
```

It may include an optional label, which by default is "Drivers License Number".

```html
<drivers-license-input label="Drivers License"></drivers-license-input>
```

## Json File Referred

Below is the Json file that is used in the element.

<https://github.com/adambullmer/USDLRegex/blob/master/regex.json>

## Validation

By default, the drivers license number is considered to be a US drivers license number, and will be validated according to the state that is selected. If you want to customize the input for a different country, change the json file with the desired country.

```html
<drivers-license-input auto-Validate></drivers-license-input>
```

The input is by using the auto-validate and required attributes. For manual validation, the element also has a validate() method, which returns the validity of the input as well sets any appropriate error messages and styles. auto-validate and required attributes can be changed as shown below.

```html
<drivers-license-input required auto-validate></drivers-license-input>
```

## Enable Drivers License only if a state is selected

To allow Drivers License to be entered only if a state is selected by setting the 'disabled' property as shown below

```html
<drivers-license-input auto-Validate disabled></drivers-license-input>
```

## License

Licensed under [Apache 2.0](LICENSE).