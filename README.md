# remify()

Simple set of Sass mixin and function to quickly convert pixels to rems.
This solution assumes that baseline is 10px, you can override that easily
by changing the `baseline-px` value in the `_remify.scss` file to the `remify()` function.

## Usage

- Quick, one-off pixels to rem value conversion

    font-size: remify(12px);

- Converting entire property

    margin-right: remify(0 20px 20px 0);

- Converting entire property with a pixel fallback for older browsers
    
    @include rem('margin-right', 0 20px 20px 0);
