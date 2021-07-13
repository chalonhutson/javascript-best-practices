1. JavaScript Integrity Checks
As a frontend developer, you may have used <script> tags to import third-party libraries. Have you thought about the security risks of doing so?
What if the third-party resource has been tampered with?
Yes, these are things that can happen when you render external resources on your site. As a result, your site may face a security vulnerability.
As a safety measure for this, you can add an integrity (also known as Subresource integrity — SRI) code to your script as follows.

2. Frequent Tests for NPM Vulnerabilities
I hope all of you know that we can use npm audit command to detect vulnerabilities for all installed dependencies. It provides vulnerability reports and provides fixes for them. But how often do you do that?
Unless we automate it, these vulnerabilities will stack up, making it difficult to fix them. Remember, some of them could even be critical, allowing severe exploits.
As a solution, you can run NPM in your CI for each pull request to identify vulnerabilities. Therefore, you can prevent any vulnerabilities from going unnoticed.

3. Sort div Tags

It's common to see multiple div tags closing at the bottom of a page. While divs are cleaner than tables, leaving them unsorted only results in a mess that is hard to clean up. Indentation is a good way to organize tag closes.

However, the best way to organize your div tags is to comment on which one you're closing. For example, adding a comment such as <!--#header -- > helps the reader understand which tag you're closing.

4. Use CSS Resets
CSS resets are a common practice in web development, but it's surprising how many beginner developers neglect to do this. The result is cross-browser rendering issues that destroy UX.

A CSS reset removes individual styling from all elements, and this leaves no room for browsers to override your style element with their defaults.

5. Avoid @import
@import was a popular choice for many developers when it came to importing CSS files. Including a stylesheet into another is easy with this directive. Alternatively, CSS files can be included in HTML documents as well.

However, as browsers drop default import support, developers have to find other ways to include external HTML files within the main file. Renaming the external HTML file extension to .shtml and using server-side includes (SSI) within the HTML is the best approach. Note that the file with the SSI command must be named with the shtml extension.

6. Conditional Commenting
Microsoft has announced the end of support for Internet Explorer which will make this requirement redundant in a few years. However, for now, it still exists and this means developers have to account for web pages being displayed on this obsolete browser.

There are hacks you can use to customize your code, but the problem is that CSS validation fails. Instead, use conditional comments to target particular versions of Internet Explorer.

7. Block scored declarations
Since the inception of the language, JavaScript developers have used var to declare variables. The keyword var has its quirks, the most problematic of those being the scope of the variables created by using it.
Since variables defined with var are not block-scoped, redefining them in a narrower scope affects the value of the outer scope.
Now we have two new keywords that replace var, namely let and const that do not suffer from this drawback.
const and let differ in the semantics that variables declared with const cannot be reassigned in their scope. This does not mean they are immutable, only that their references cannot be changed.

8. Generally when a WebSocket connection is established, a server could time out your connection after 30 seconds of inactivity. The firewall could also time out the connection after a period of inactivity.

To deal with the timeout issue you could send an empty message to the server periodically. To do this, add these two functions to your code: one to keep alive the connection and the other one to cancel the keep alive. Using this trick, you’ll control the timeout.

9. React is booming
The popularity of React has been growing over the past few years and does not show any signs of stopping.
This library came into being in 2011. At that time, Facebook needed a specific tool for maintaining the rapidly evolving traffic for their services. So they introduced a solution called FaxJS. It can be seen as the early-stage prototype for React.

10. Vue is evolving further
2020 was marked with the long-expected release of Vue.js — 3.0. What did it bring? We should mention the boosted apps’ performance and smaller bundle sizes. Also, we saw significant improvement in TypeScript support.
Let’s list up the key Vue advancements that will impact JavaScript trends in 2021 and further.
Improved performance;
Support of large-scale projects;
TypeScript integration;
Layered modules.