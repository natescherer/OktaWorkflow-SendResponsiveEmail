# Okta Workflow: Send Responsive Email

An Okta Workflow to send a responsive HTML email.

This project is unofficial and is neither developed nor supported by Okta.

## Installing

To install this workflow, follow these steps:

1. Download the latest release from [releases](releases)
1. Create a new folder in Okta Workflows
1. Import the `sendResponsiveEmail.folder` file into the new folder
1. Open each flow in the folder and connect the app actions to the pre-configured actions for your environment (see [here](https://help.okta.com/en/prod/Content/Topics/Workflows/workflow-connect-your-applications.htm) if you have not yet configured connections)
1. Enable all flows
1. Test
1. Once the testing is complete, you can remove the `Send Test Email` flow, as it is just to demostrate the process. The `Build Responsive Email` flow can be called from whatever flows you wish.

## Customizing

The `Build Responsive Email` flow can be customized in several ways:

- Color Scheme
  - The `Define Color Scheme` step can be customized by replacing the colors with the hex color values of your choice. [Here is a useful color picker](https://www.w3schools.com/colors/colors_picker.asp) if you need it.
- Fonts
  - The `Define Font Scheme` step can be customized by replacing the default fonts with fonts of your choice. It is strongly recommended that you only use web safe fonts to ensure your emails will render properly across mail clients. A list of web safe fonts can be be found [here](https://www.smartrmail.com/blog/email-safe-fonts-web-safe-fonts-for-email-explained/).

## Using

The `Header Text` and `Footer Text` inputs to the `Build Responsive Email` flow should be a single line of plain text.

The `Body` input can contain whatever HTML you wish, and has the additional option of including a button through the use of the following pseudocode:

```HTML
<!-- Button Link -->https://okta.com<!-- Button Text -->CLICK HERE<!-- Button End -->
```

## Authors

**Nate Scherer** - *Initial work* - [natescherer](https://github.com/natescherer)

## License

This project is licensed under The MIT License - see [LICENSE](LICENSE) for details.

## Acknowledgements

[leemunroe](https://github.com/leemunroe/responsive-html-email-template) - The core email formatting of PoshEmail is built on leemunroe's "Really Simple Free Responsive HTML Email Template".
