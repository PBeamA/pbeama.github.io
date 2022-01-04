---
title: Resources
icon: fa fa-book
math: true
order: 4
---


### [Resources](https://github.com/PBeamA/Resources)

#### Assignment Cover Sheet:
<object data="https://github.com/PBeamA/Resources/raw/master/Academia/CoverSheet.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://github.com/PBeamA/Resources/raw/master/Academia/CoverSheet.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://github.com/PBeamA/Resources/blob/master/Academia/CoverSheet.pdf">Download PDF</a>.</p>
    </embed>
</object>

<!--
## [$\LaTeX$](/LaTeX/)
-->
### [AutomatingLaTeX](https://github.com/PBeamA/AutomatingLaTeX)


### Modified Chirpy Template -- This site's template...
[Template Link](https://github.com/PBeamA/chirpy-starter-modified/generate)

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
