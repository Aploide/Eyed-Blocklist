# Eyed Blocklist

## Version 2.20

This blocklist is officially used by the **[Eyed Out Browser](https://apps.apple.com/app/eyed-out-private-web-browser/id6475011990)**, a private web browser available on iOS devices. It's compatible with the WebKit engine, meaning it works seamlessly within the browsers or applications utilizing WebKit.

## Features

- **Ad Blocking**: Blocks intrusive advertisements across various websites, providing a cleaner and more enjoyable browsing experience.
  
- **Tracker Blocking**: Prevents tracking scripts and cookies from collecting your data and monitoring your online activity, enhancing your privacy.
  
- **Optimized for WebKit**: The blocklist uses JSON-based instructions specifically tailored for the WebKit engine, ensuring maximum compatibility and performance.
  
- **Lightweight and Efficient**: Carefully curated to minimize resource usage while maintaining high effectiveness in blocking unwanted content.

## Installation and Usage

The **Eyed Blocklist** is automatically included and updated within the **[Eyed Out Browser](https://apps.apple.com/app/eyed-out-private-web-browser/id6475011990)**. 
If you are using this browser, you do not need to take any additional steps. 
The blocklist will function in the background, providing you with a smoother and more private browsing experience.

### Manual Installation (For WebKit-Based Browsers)

If you are using another WebKit-based browser or application, you can manually install the Eyed Blocklist by following these steps:

1. Download the latest version of the blocklist.
2. Follow the instructions specific to your browser or application for importing custom blocklists.
3. Ensure that the blocklist is active and configured correctly within your browser's settings.

## Blocklist Format

The Eyed Blocklist is provided in a JSON format that is compatible with WebKit-based browsers. The blocklist entries are structured to specify the elements, domains, and scripts that need to be blocked. Here’s a simplified example of the structure:

```json
{
  "trigger": {
    "url-filter": ".*",
    "resource-type": ["image", "script", "stylesheet"]
  },
  "action": {
    "type": "block"
  }
}
```

- **trigger**: Defines the conditions under which the block action should be applied. This could include specific URL patterns, resource types, or other conditions.
  
- **action**: Specifies the action to be taken when the trigger conditions are met. In most cases, this will be a "block" action to prevent the resource from loading.

For more details on the structure and how to customize the blocklist, refer to the [WebKit Content Blocker Documentation](https://webkit.org/blog/3476/content-blockers-first-look/).

## Contributing

We welcome contributions to improve and expand the Eyed Blocklist. If you find a domain or resource that should be blocked but isn't currently covered, feel free to submit an issue or a pull request.

### How to Contribute

1. Fork the repository.
2. Make your changes or additions to the blocklist.
3. Submit a pull request with a detailed explanation of your changes.

Please ensure that any contributions follow the JSON structure and maintain compatibility with WebKit.

## License

The Eyed Blocklist is licensed under the **Mozilla Public License 2.0**. See the [LICENSE](#) file for more details.

## Support

For any issues, questions, or suggestions, feel free to open an issue on this repository or contact us through our email [here](mailto:yo@aploide).