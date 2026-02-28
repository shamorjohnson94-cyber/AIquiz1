# AIquiz1
Name: Shamor Johnson
Tools used: ChatGPT, Colab, Browser

Q1:
- Key finding (2-4 sentences):
The scatter plot demonstrates a strong positive correlation between study hours and exam scores. As the number of hours studied increases, exam performance consistently improves. The upward trendline confirms a linear relationship, indicating that increased study time is associated with higher academic achievement.

- Outlier:
There were no major outliers, although the lowest study-hour data point had a slightly lower score compared to the trendline.

Q2:
- What was broken:
The webpage layout did not adjust properly on smaller screen sizes.
- What I changed:
I added a viewport meta tag and implemented responsive CSS using max-width: 100% and height: auto.

Q3:
Prompt 1 (plan, no code):
I asked ChatGPT for a plan to implement responsive breakpoints and hero behavior, and I accepted using standard breakpoints (mobile, tablet, desktop) and stacking the hero vertically on small screens, but I rejected drastic font-size changes as they reduced readability. 

Response snippet:
I asked ChatGPT for a plan to implement responsive breakpoints and hero behavior, and I accepted using standard breakpoints (mobile, tablet, desktop) and stacking the hero vertically on small screens, but I rejected drastic font-size changes as they reduced readability. I ran into a bug where the hero overflowed on mobile (.hero { display: flex; flex-direction: row; gap: 2rem; }), and ChatGPT suggested using flex-direction: column in a media query, which I implemented with @media (max-width: 480px) { .hero { flex-direction: column; } }. I verified the fix on 375px, 768px, and 1200px viewports, confirming the hero stacked properly on mobile and aligned correctly on larger screens.

Accepted:
- Overall page structure
- Navigation layout

Rejected:
- Inline styling because it reduced maintainability

Prompt 2 (debug):
 I ran into a bug where the hero overflowed on mobile (.hero { display: flex; flex-direction: row; gap: 2rem; })
Response snippet:
My image is not showing on my gallery page even though the file is uploaded. Here is my HTML code. What is wrong?

What I verified:
- viewport sizes tested: desktop, tablet, mobile
- what I checked visually: image scaling, spacing consistency, header and footer formatting

Q4:
- Chart caption:
This chart shows a clear positive relationship between the number of hours studied and exam scores, with scores increasing as study time increases. Based on this trend, encouraging students to dedicate more consistent study hours could improve overall academic performance.

- Decision based on chart:
Encourage structured and increased study time to improve exam outcomes.
