# Text Blocks with Format Specifiers

![j](https://user-images.githubusercontent.com/116082827/236695461-2ceeba9c-42cb-4787-bcb8-e1fca654074b.png)


Java 16 introduced an enhancement to text blocks that allows for the inclusion of format specifiers within the text block. This feature allows for the easy formatting of text within the text block.



Example:





String message = """

                  Dear %s,

                  

                  Thank you for your recent order.

                  Your order number is %d.

                  

                  Regards,

                  The Store

                  """;

String formatted = String.format(message, "John", 12345);

System.out.println(formatted);
