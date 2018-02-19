# to-fixed-of-beast
Created a getExponentialForm(value,precision) function which gets called by toFixed to generate the exponential form.

Following is the implementation details of getExponentialForm(value,precision)
If the precision is positive 
  - Identifies the new decimal position 
  - moves the decimal point to the right based on the precision value
  - pads 0 if the precision value greater than the length of the value as a string

If the precision is negative
  - reverses the string
  - Identifies the new decimal position 
  - moves the decimal point to the right based on the precision value
  - reverses the string to bring it back to it's original value
  - removes any leading 0 in the whole number part of the string 


