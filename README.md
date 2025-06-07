# Evaluating Ad Blockers for Privacy


This research project aimed to quantitatively evaluate the effectiveness of popular ad blockers in enhancing user privacy and improving browser performance across major web browsers.

**Objective**:
To measure how well four popular ad blockers—AdBlock, AdBlock Plus, uBlock Origin, and Ghostery—perform in terms of:

Blocking third-party trackers
Improving page load times
Reducing unnecessary network requests
Maintaining functional website integrity

**Methodology**:
Used Selenium to automate visits to the top 100 websites from the Fortune 250 list.
Deployed BrowserMob Proxy to capture network traffic in HAR files.
Tested on Google Chrome, Mozilla Firefox, and Microsoft Edge with each blocker installed.
Parsed over 1,200 HAR files using a custom Python parser, extracting metrics like:
Number of third-party requests
Unique third-party domains
Average and 95th percentile request durations
Total page load times

**Key Findings & Conclusion**:

uBlock Origin emerged as the top performer, blocking ~94% of third-party trackers and improving page load time by an average of 25% over no blocker and 12% over AdBlock Plus.
Chrome and Edge, both Chromium-based, showed similar network behaviors and blocking patterns.
Firefox exhibited more variability (~11%) in blocking due to differences in its rendering engine and extension APIs.
Ghostery had the highest chance of functional breakage—7% of sites showed broken layouts or missing elements due to overblocking.
This research revealed that not all ad blockers are created equal, and choosing the right tool can significantly impact both privacy and browsing experience.

