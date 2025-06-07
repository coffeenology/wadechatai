# AI Multi-Character Roleplay Blocklist

This repository hosts a blocklist of domains for NSFW AI-driven multi-character roleplay (MCRP) platforms, designed for DNS filtering tools like NextDNS, Pi-hole, or AdGuard. The list targets websites offering unfiltered or 18+ roleplay content, making them unsuitable for kids, while striving to avoid false positives.

## Purpose

The blocklist enables users, parents, or administrators to restrict access to NSFW AI MCRP platforms, promoting safer internet browsing. It is released into the public domain under the Creative Commons CC0 1.0 Universal license, allowing unrestricted use, modification, and distribution.

## Blocklist File

- **File**: `chatai_blocklist.txt`
- **Format**: Plain text, one domain per line (e.g., `janitorai.com`)
- **Content**: Domains of NSFW AI MCRP platforms, such as `spicychat.ai` and `venus.chub.ai`

## How to Use

### 1. Obtain the Blocklist URL

- Copy the raw URL of the blocklist file:
Replace `[your-username]` and `[your-repo]` with your GitHub username and repository name.
    
    ```
    https://github.com/coffeenology/wadechatai/blob/main/chat_blocklist.txt
    
    ```
    

### 2. Add to DNS Filtering Tool

### NextDNS

1. Log in to your NextDNS account at [nextdns.io](https://nextdns.io/).
2. Navigate to the **Privacy** tab and select **Blocklists**.
3. Click **Add a blocklist**.
4. Paste the raw URL of the blocklist and click **Add**.
5. Save changes. The blocklist should take effect immediately, but you may need to flush your DNS cache (e.g., `ipconfig /flushdns` on Windows).

### Pi-hole

1. Access your Pi-hole web interface.
2. Go to **Adlists** under **Group Management**.
3. Paste the raw URL of the blocklist in the **Address** field.
4. Click **Add** and then **Update Gravity** to apply the list.

### AdGuard Home

1. Log in to your AdGuard Home dashboard.
2. Go to **Filters** > **DNS blocklists**.
3. Click **Add blocklist** and paste the raw URL of the blocklist.
4. Save and refresh the filter to apply the changes.

### 3. Test the Blocklist

- Try accessing a domain from the blocklist (e.g., `janitorai.com`).
- Verify that access is blocked. If not, check your DNS filter’s configuration or flush your DNS cache.
- Review your DNS filter’s logs to detect any false positives (legitimate domains blocked incorrectly).

### 4. Report Issues

- If a domain should be added or removed, submit an issue or pull request on this repository.
- Include details, such as the domain, why it should be included/excluded, and evidence of NSFW AI MCRP content.

## Updating the Blocklist

- The blocklist is periodically updated to add new NSFW AI MCRP platforms or remove outdated domains.
- Ensure your DNS filter fetches the raw URL regularly to stay current (most tools handle this automatically).

## Notes

- **False Positives**: Test thoroughly to prevent blocking legitimate websites. Report issues promptly.
- **Privacy**: The blocklist contains only domain names and collects no user data.
- **Compatibility**: Compatible with any DNS filter supporting plain-text domain lists.

## License

This project is dedicated to the public domain under the [Creative Commons CC0 1.0 Universal (CC0)](https://creativecommons.org/publicdomain/zero/1.0/) license. You are free to use, modify, distribute, and incorporate the blocklist for any purpose, including commercial use, without restriction or attribution. See the `LICENSE` file for details.
