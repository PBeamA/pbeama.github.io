---
title: Resources
icon: fa fa-book
math: true
order: 4
---


### [Resources](https://github.com/PBeamA/Resources)
- Courses...
  - [Assignment Cover Sheet](https://github.com/PBeamA/Resources/blob/master/Academia/CoverSheet.pdf)
  - [MFinc Template (MSWord)](https://github.com/PBeamA/OtagoTemplates/blob/main/MFincTemplate.docx)
  - [Paper Template (MSWord)](https://github.com/PBeamA/OtagoTemplates/blob/main/PaperTemplate.docx)
- LaTeX
  - [Templates](https://github.com/PBeamA/Resources/tree/master/LaTeX/Templates)
    - [Paper Template](https://github.com/PBeamA/Resources/blob/master/LaTeX/Templates/PaperTemplate.pdf)
    - [Presentation (Beamer) Template](https://github.com/PBeamA/Resources/blob/master/LaTeX/Templates/BeamerTemplate.pdf)
  - [References](https://github.com/PBeamA/Resources/tree/master/LaTeX/References)
    - [American Finance Association (AFA) Style](https://github.com/PBeamA/Resources/blob/master/LaTeX/References/ReferencesAFA.tex)
    - [American Psychological Association (APA) Style](https://github.com/PBeamA/Resources/blob/master/LaTeX/References/ReferencesAPA.tex)

<!--
#### Assignment Cover Sheet:
<object data="https://github.com/PBeamA/Resources/raw/master/Academia/CoverSheet.pdf" type="application/pdf" width="700px" height="700px">
</object>
-->

<!--
## [$\LaTeX$](/LaTeX/)
-->
### [AutomatingLaTeX](https://github.com/PBeamA/AutomatingLaTeX)
A step towards getting [knitr](https://github.com/yihui/knitr) for MATLAB...
- MATLAB to LaTeX
Getting LaTeX to read MATLAB output efficiently
- Clean LaTeX
Remove MATLAB integration to make the LaTeX files standalone



### Modified Chirpy Template -- This site's template...[^1]
[Template Link](https://github.com/PBeamA/chirpy-starter-modified/generate)


[^1]: a slightly older template... If you'd like the new one, just let me know

<!--
## Appendix
Add ```\preappendix``` before and ```\postappendix``` after.

For sections in the appendix use ```\subsection``` instead of ```\section```.

# MATLAB
## Save figure as PDF (and PNG)
```
function saveasPDF(h, filename)
% Eg. saveasPDF(gcf, sprintf('Filename'))
fig = h;
set(fig,'PaperPositionMode', 'auto');
fig_pos = fig.PaperPosition;
fig.PaperSize = [fig_pos(3) fig_pos(4)];


title([])
set(gca, 'LooseInset', get(gca, 'TightInset'));

print(fig, filename, '-dpdf', '-bestfit', '-painters')
print(fig, regexprep(filename, '.pdf', '.png'), '-dpng', '-r600')

end
```

## Shade $x$-axis
```
function shadex(x1, x2)
% Shades current figure from x1 to x2
hold on
ylimits = get(gca, 'ylim'); % Get y axis limits
 
colour = [0.4, 0.4, 0.4];   % Grey
p = fill([x1, x2, x2, x1], sort([ylimits, ylimits]), colour);
set(p, 'FaceAlpha', 0.25, 'EdgeColor', 'none');
 
end
```
<sup>Note: Works with MATLAB R2017a and not 2016a</sup>
-->
