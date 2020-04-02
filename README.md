# Accordion Dynamic Content

## Sample Description

The Accordion component supports to load content as dynamically using `ContentTemplate` property and prefered content can be passing through `RenderFragment`.

> ContentTemplate property supports RenderFragment type to render content.

## Steps to create Dynamic Accordion Content

  1. Create a blazor application using this [getting started](https://blazor.syncfusion.com/documentation/getting-started/server-side-blazor/) link.

  2. Define the Accordion content as `RenderFragment` type for dynamic loading. Refer the below code for that

  ```
  @using Syncfusion.Blazor.Navigations

<SfAccordion>
    <AccordionItems>
        <AccordionItem>
            <HeaderTemplate>
                <div>Margeret Peacock</div>
            </HeaderTemplate>
            <ContentTemplate>
                Margeret Peacock was born on Saturday , 01 December 1990. Now lives at Coventry House Miner Rd., London,UK. Margeret Peacock holds a position of Sales Coordinator in our WA department, (Seattle USA). Joined our company on Saturday , 01 May 2010
            </ContentTemplate>
        </AccordionItem>
        <AccordionItem>
            <HeaderTemplate>
                <div>Laura Callahan</div>
            </HeaderTemplate>
            <ContentTemplate>
                Laura Callahan was born on Tuesday , 06 November 1990. Now lives at Edgeham Hollow Winchester Way, London,UK. Laura Callahan holds a position of Sales Coordinator in our WA department, (Seattle USA). Joined our company on Saturday , 01 May 2010
            </ContentTemplate>
        </AccordionItem>
        <AccordionItem>
            <HeaderTemplate>
                <div>Albert Dodsworth</div>
            </HeaderTemplate>
            <ContentTemplate>@DynamicContent</ContentTemplate>
        </AccordionItem>
    </AccordionItems>
</SfAccordion>

@code {
    public RenderFragment DynamicContent = builder =>
    {
        builder.AddContent(1, "Albert Dodsworth was born on Thursday, 19 October 1989.Now lives at 4726 - 11th Ave.N.E., Seattle, USA.Albert Dodsworth holds a position of Sales Representative in our WA department, (Seattle USA).Joined our company on Friday, 01 May 2009");
    };
}

   3. Simply press `F5` to run the application.

  ```

