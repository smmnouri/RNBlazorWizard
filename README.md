RNBlazorWizard

A Beautiful, Lightweight Blazor Wizard Component for .NET 8

**Introduction**

RNBlazorWizard is a user-friendly, feature-rich Blazor component designed to streamline the creation of multi-step wizards within your .NET 8 applications.
It boasts a lightweight design, stunning aesthetics, and robust functionality, making it an exceptional choice for enhancing your user experience.
Key Features

Step-by-Step Navigation: Guide users through a clear progression of steps, ensuring an intuitive and organized interaction.
Submission Handling: Capture and process user input at each wizard step, allowing you to collect and validate data effectively.
Customizable Appearance: Tailor the component's look and feel to seamlessly integrate with your application's design aesthetic.
Loading Integration (Optional): Optionally incorporate loading indicators or custom toast notifications to provide visual feedback during data processing or step transitions.
Future-Proof for .NET 8: Developed specifically for .NET 8, ensuring compatibility and leveraging the latest Blazor enhancements.
Usage

**Basic Usage:**


<Wizard>
    <WizardStep Title="General Info" Submit="@SubmitStep1">
        <Step1 @ref="@step1"></Step1>
    </WizardStep>
    <WizardStep Title="Personal Info" Submit="@SubmitStep2">
        <Step2 @ref="@step2"></Step2>
    </WizardStep>
    <WizardStep Title="Bank Info" Submit="@SubmitStep3">
        <Step3 @ref="@step3"></Step3>
    </WizardStep>
    <WizardStep Title="Confirmation" Submit="@SubmitStep4">
        <Step4 @ref="@step4"></Step4>
    </WizardStep>
</Wizard>
**Use code with caution.**

Replace Step1, Step2, Step3, and Step4 with your custom component names representing the content for each wizard step.
Define methods like SubmitStep1, SubmitStep2, etc., in your code-behind file or Razor component to handle form submissions at each step.
**Note** : in dotnet 8 , @rendermode InteractiveServer !! important
**Explanation:**
The Wizard component encapsulates the overall wizard structure.
Each WizardStep represents a distinct step in the wizard flow.
The Title property sets the label displayed for each step.
The Submit event handler is bound to a method that handles form submission or any actions specific to that step.
You can reference child components within each WizardStep to create the content for each step. In this example, Step1, Step2, etc., are assumed to be your custom components that render the step content.
By providing references (using @ref="@step1") to these child components, you can potentially access their state or properties within your submit methods.
Additional Notes:

Remember to create your custom components (Step1, Step2, etc.) to handle the specific content and logic for each step.
Customize the component's appearance (styling) as needed to match your application's design.
This revised section provides a clear explanation of how to use your code snippet and integrate it with RNBlazorWizard, making it easier for users to understand and implement it in their projects.
