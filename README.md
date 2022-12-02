# Introduction
Validation of InputNumber and model data annotation doesn't work as expected.

# Reproduce bug by steps and explanation
## Step 1 - Clear endered data from InputText
Nothing to exmlain jet.
## Step 2 - Focus out from InputText
Generic error message is shown, but it should be error message defined by RequredAttribute.
## Click on "+" or "-" button
InputNumber is still marked with error, but it should't because now it has value.
(EditContextRef.GetValidationMessages() still holds the same error)
# Example which works fine
While (int)Counter does not work as expected, (int?)Counter works just fine.
Not working and working examples are shown at Index page.


