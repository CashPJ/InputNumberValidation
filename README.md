# Introduction
Validation of InputNumber and model data annotation doesn't work as expected.

# Reproduce bug by steps and explanation
## Step 1 - Clear endered data from InputText
Nothing to exmlain jet.

![step1](https://user-images.githubusercontent.com/80749332/205308614-9f26a2e1-cabd-43e7-8d7b-ba8154e12173.png)

## Step 2 - Focus out from InputText
Generic error message is shown, but it should be error message defined by RequredAttribute.

![step2](https://user-images.githubusercontent.com/80749332/205308663-474cb470-bc10-423a-b4e8-b7002654f7d9.png)

## Step 3 - Click on "+" or "-" button
InputNumber is still marked with error, but it should't because now it has value.
(EditContextRef.GetValidationMessages() still holds the same error)

![step3](https://user-images.githubusercontent.com/80749332/205308706-a453995a-4158-4435-b2e0-eaae47a426a4.png)

# Example which works fine
While (int)Counter does not work as expected, (int?)Counter works just fine.
Not working and working examples are shown at Index page.


