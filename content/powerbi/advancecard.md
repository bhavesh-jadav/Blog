---
title: "Advance Card - A Power BI Custom Visual"
date: 2018-06-03T15:01:15+05:30
draft: false
categories: 
    - "Power BI"
tags: 
    - "Power BI"
    - "Custom Visual"
---

Advance Card is a Power BI custom visual with more features than default card visual present in Power BI. It is built to overcome some of the limitation of the default card visual in Power BI. Below you will find some of the features of Advance Card.

**Prefix and Postfix Labels**  
You can add prefix and postfix label along with category label. Prexfis and postfix labels are useful to append text to begining and end of datalabel respectively. This is esepcially useful in live connection. You can achieve similar result with DAX and default card visual but for that you will have to write multiple DAX query for multiple card and DAX does not support formatting. With prefix and postfix label you can also customize size, color and other properties of the text which is not possible in DAX as of now.
<figure>
  <img class = "center" src = "/gifs/prefix_postfix.gif" alt = "Prefix and Postfix Demo"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">Prefix and postfix label in Advance Card visual</figcaption>
</figure>

**Conditional Formatting**  
This is one of the important feature of Advance card visual. You can specify different conditions and based on that condition it will change color of either prefix, postfix, data label, category label or all them based on which label you want to apply conditional formatting. Some scenario where it can be useful are:  

* Showing states: value > 90 then green | value > 50 then yellow | value > 0 then red
* Range formatting: If value is between 10 and 30 then show green else show red.
* Comparing two or more values(through DAX): If actual > target then red else green

<figure>
  <img class = "center" src = "/gifs/conditional_format.gif" alt = "Conditional Formatting Demo"></img>
  <figcaption class = "center" style = "margin-top: 5px; text-align: center;">Conditional formatting in Advance Card visual</figcaption>
</figure>

**Tooltip**  
You can show data in form of tooltip on Advance Card which is not possible with default card visual. This useful if you want to show custom information, extra data in form of tooltip.

<figure class = "center">
  <img src = "/gifs/tooltip.gif" alt = "Tooltip Demo"></img>
  <figcaption style = "margin-top: 5px; text-align: center;">Tooltip in Advance Card visual</figcaption>
</figure>

**Stroke (Border) Formatting**  
This feature is is useful to make card more visually attractive. You can change stroke(border) size, color, type, corner radius etc.

<figure class = "center">
  <img src = "/gifs/stroke.gif" alt = "Stroke Formatting Demo"></img>
  <figcaption style = "margin-top: 5px; text-align: center;">Stroke formatting in Advance Card visual</figcaption>
</figure>


**Features Comparison**

<table>
  <thead>
    <tr>
      <th>Features</th>
      <th>Advance Card Visual</th>
      <th>Default Card Visual</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td style = "text-align: center;">
            Data label formatting
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Category Label Formatting
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Prefix and postfix label
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">❌</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Conditional Formatting
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">❌</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Conditional formatting based on other measure
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">❌</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Tooltip support
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">❌</span>
            </font>
        </td>
    </tr>
    <tr>
        <td style = "text-align: center;">
            Stroke or border manipulation
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">✔</span>
            </font>
        </td>
        <td style = "text-align: center;">
            <font face="Segoe UI Emoji,sans-serif" size="4" color="#191E3F">
                <span style="font-size:14pt;">❌</span>
            </font>
        </td>
    </tr>
  </tbody>
</table>

**Resources**  
Download Advance Card custom visual and sample report [from github](https://github.com/bhavesh-jadav/Advance-Card/releases)  
Detailed documentation available at [Github Wiki](https://github.com/bhavesh-jadav/Advance-Card/wiki)  
Privacy Policy available at [Power BI Custom Visual Privay Policy]({{< ref "powerbi-privacy-policy.md" >}})  
