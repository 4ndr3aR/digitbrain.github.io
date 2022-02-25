<style>
  .md-content__button {
    display: none;
  }
</style>
# Outputs Fields

**This information is also available in [table format](/tables/outputs/)**


## Available Fields 

The metadata specification for a DIGITbrain Outputs
has these sections:

- [Outputs](#outputs)


### Outputs


`Key`{ #key }
:   **Optional**-*string*- Group key (eg. type and name) of the output

`Name`{ #name }
:   **Optional**-*string*- Human-readable name of the output

`Dimensions`{ #dimensions }
:   **Optional**-*number*- Number of dimensions of the output (i.e. scalar, vector field)

`Is-continuous`{ #is-continuous }
:   **Optional**-*boolean*- Continuous or discreet output

`Units`{ #units }
:   **Optional**-*obj (see subkeys below)*- Values related to the output measurement units

    `Unit`{ #unit }
:   **Optional**-*string*- Units of the output (e.g Pa, m/s, etc…)

    `Exponent`{ #exponent }
:   **Optional**-*array of number*- eg. exponents for kg (SI) {1, -2, 0, 0, 0, 0, 1}

    `Offset`{ #offset }
:   **Optional**-*number*- scale offset if needed (e.g. K to C conversion)

    `Scale`{ #scale }
:   **Optional**-*number*- Order of magnitude of the measurement unit scale e.g. Scale is equal to 10^-3 for values expressed in mm

`Default-value`{ #default-value }
:   **Optional**-*number*- Default value for the output

`Ranges`{ #ranges }
:   **Optional**-*array of number*- Max and min value of the output
