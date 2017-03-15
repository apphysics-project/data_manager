# Objects

## Symbol

1. *id*
1. *names*
1. *texSyntax*

Examples: mu, tau, sum

## Property

1. *id*
1. *name*
1. *description*

Examples: Mass, Velocity, Acceleration

## UnitSystem

1. *id*
1. *names*
1. *acronym*
1. *description*

Examples: International System of Units, Imperial Units

## Unit

1. *id*
1. *name*
1. *pluralName*
1. *[symbol](#symbol)*
1. *description*
1. *isScalar*
1. *[property](#property)*
1. *[unitSystem](#unitsystem)*

Examples: Metre, Kilogram, Second

## ScaledUnit *extends [Unit](#unit)*

1. *[baseUnit](#unit)*
1. *scale*

Examples: Kilometre, Gram, Millisecond

## DerivedUnit *extends [Unit](#unit)*

1. *[baseUnits](#unit)*
1. *expressions*
1. *[property](#property)*

Examples: Metre per second, Newton, Joule

## Conversion

1. *id*
1. *[unit](#unit)*
2. *[toUnit](#unit)*
3. *conversionScale*

Example: Yard to Metre - 0.9144

## Major Area

1. *id*
1. *names*
1. *description*

Example: Classical, Modern

## Branch

1. *id*
1. *names*
1. *description*
1. *[majorArea](#major-area)*

Examples: Kinematics, Dynamics, Acoustics

## Category

1. *id*
1. *names*
1. *description*
1. *[branch](#branch)*

Examples: Newton's Law of Motion, Special Theory of Relativity

## SubCategory *extends Category*

1. *[Category](#category)*

Examples: Newton's First Law, Reference Frames

## Variable

1. *id*
1. *[symbol](#symbol)*
1. *description*
1. *[property](#property)*

Example: m in F = ma

## Equation

1. *names*
1. *description*
1. *[variables](#variable)*
1. *equation*

Example: Newton's First Law Equation
 
 Choose Files Choose Files
