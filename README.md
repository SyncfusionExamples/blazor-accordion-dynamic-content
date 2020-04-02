# Blazor-Tabs-Select-Tab Item

## Sample Description

The Blazor Tab component supports to select specific Tab item using `SelectedItem` property otherwise the first Tab item has been selected by default.

## Steps to select specific Tab item

  1. Create a blazor application using this [getting started](https://blazor.syncfusion.com/documentation/getting-started/server-side-blazor/) link.

  2. Define the Tab with `SelectedItem` property to select the particular Tab item. Refer the below code for that

  ```
  @using Syncfusion.Blazor.Navigations

<SfTab SelectedItem="2">
    <TabItems>
        <TabItem>
            <ChildContent>
                <TabHeader Text="HTML"></TabHeader>
            </ChildContent>
            <ContentTemplate>
                <div>HyperText Markup Language, commonly referred to as HTML, is the standard markup language used to create web pages. Along with CSS, and JavaScript, HTML is a cornerstone technology, used by most websites to create visually engaging web pages, user interfaces for web applications, and user interfaces for many mobile applications.[1] Web browsers can read HTML files and render them into visible or audible web pages. HTML describes the structure of a website semantically along with cues for presentation, making it a markup language, rather than a programming language.</div>
            </ContentTemplate>
        </TabItem>
        <TabItem>
            <ChildContent>
                <TabHeader Text="Java"></TabHeader>
            </ChildContent>
            <ContentTemplate>
                <div>Java is a set of computer software and specifications developed by Sun Microsystems, later acquired by Oracle Corporation, that provides a system for developing application software and deploying it in a cross-platform computing environment. Java is used in a wide variety of computing platforms from embedded devices and mobile phones to enterprise servers and supercomputers. While less common, Java applets run in secure, sandboxed environments to provide many features of native applications and can be embedded in HTML pages.</div>
            </ContentTemplate>
        </TabItem>
        <TabItem>
            <ChildContent>
                <TabHeader Text="JavaScript"></TabHeader>
            </ChildContent>
            <ContentTemplate>
                <div>JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.[5] More recently, however, it has become common in both game development and the creation of desktop applications.</div>
            </ContentTemplate>
        </TabItem>
    </TabItems>
</SfTab>

```
  3. Simply press `F5` to run the application.