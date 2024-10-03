<!-- This snippet has the side effect of creating an empty equation block, which
takes vertical space, so include it somewhere where that space is innocuous
(e.g., after an intro paragraph.)

We don't want to include multiple such snippets (nor would it be good to have
conflicting macros), so all macros are in one place.
-->

$$
%% basic math
\gdef\intersect{\cap}
\gdef\union{\cup}
\gdef\dom{\operatorname{dom}}
\gdef\disjoint{\mathrel{\bot}}
\gdef\finto{\overset{\text{fin}}{\rightharpoonup}}

%% language
\gdef\ife#1#2#3{\text{\textbf{if} } #1 \text{ \textbf{then} } #2 \text{ \textbf{else} } #3}
\gdef\lete#1#2{\text{\textbf{let} } #1 := #2 \text{ \textbf{in} }}
\gdef\letV#1#2{&\text{\textbf{let} } #1 := #2 \text{ \textbf{in} }}
\gdef\num#1{\overline{#1}}
\gdef\true{\mathrm{true}}
\gdef\false{\mathrm{false}}
\gdef\fun#1{\lambda #1.\,}
\gdef\funblank{\fun{\_}}
\gdef\rec#1#2{\text{\textbf{rec} } #1 \; #2.\;\,}
\gdef\app#1#2{#1 \, #2}
\gdef\then{;\;}
\gdef\assert#1{\operatorname{assert} \, #1}
\gdef\val{\mathrm{val}}
\gdef\purestep{\xrightarrow{\text{pure}}}

%% hoare logic
\gdef\False{\mathrm{False}}
\gdef\True{\mathrm{True}}
\gdef\hoare#1#2#3{\left\{#1\right\} \, #2 \, \left\{#3\right\}}
\gdef\hoareV#1#2#3{\begin{aligned}%
  &\left\{#1\right\} \\ &\quad #2 \\ &\left\{#3\right\}%
  \end{aligned}}
\gdef\wp{\operatorname{wp}}
\gdef\outlineSpec#1{\left\{#1\right\}}
\gdef\entails{\vdash}
\gdef\eqnlabel#1{\:\:\text{#1}}
\gdef\lift#1{\lceil #1 \rceil}

%% separation logic
% imperative constructs
\gdef\load#1{{!}\,#1}
\gdef\store#1#2{#1 \mathbin{\gets} #2}
\gdef\free#1{\operatorname{free} \, #1}
\gdef\alloc#1{\operatorname{alloc} \, #1}
% logic
\gdef\sep{\mathbin{\raisebox{1pt}{$\star$}}}
\gdef\bigsep{\mathop{\vcenter{\LARGE\hbox{$\star$}}}}
\gdef\wand{\mathbin{\raisebox{1pt}{$-\hspace{-0.06em}\star$}}}
\gdef\emp{\mathrm{emp}}
\gdef\pointsto{\mapsto}
\gdef\Heap{\mathrm{Heap}}
\gdef\Loc{\mathrm{loc}}
$$