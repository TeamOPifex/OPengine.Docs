OPtween.h
=========

Globals
----------------
Functions
----------------
- OPfloat OPtween_linear ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x<br />

- OPfloat OPtween_quadraticEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x^2<br />

- OPfloat OPtween_quadraticEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = -x^2 + 2x<br />

- OPfloat OPtween_quadraticEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)((2x)^2) ; [0, 0.5)<br />y = -(1/2)((2x-1)*(2x-3) - 1) ; [0.5, 1]<br />

- OPfloat OPtween_cubicEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x^3<br />

- OPfloat OPtween_cubicEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = (x - 1)^3 + 1<br />

- OPfloat OPtween_cubicEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)((2x)^3) ; [0, 0.5)<br />y = (1/2)((2x-2)^3 + 2) ; [0.5, 1]<br />

- OPfloat OPtween_quarticEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x^4<br />

- OPfloat OPtween_quarticEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = 1 - (x - 1)^4<br />

- OPfloat OPtween_quarticEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)((2x)^4) ; [0, 0.5)<br />y = -(1/2)((2x-2)^4 - 2) ; [0.5, 1]<br />

- OPfloat OPtween_quinticEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x^5<br />

- OPfloat OPtween_quinticEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = (x - 1)^5 + 1<br />

- OPfloat OPtween_quinticEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)((2x)^5) ; [0, 0.5)<br />y = (1/2)((2x-2)^5 + 2) ; [0.5, 1]<br />

- OPfloat OPtween_sineEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : quarter cycle sin(x)<br />

- OPfloat OPtween_sineEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : quarter cycle offset sin(x)<br />

- OPfloat OPtween_sineEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : half sine(x)<br />

- OPfloat OPtween_circularEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : shifted quadrant IV of unit circle<br />

- OPfloat OPtween_circularEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : shifted quadrant II of unit circle<br />

- OPfloat OPtween_circularEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)(1 - sqrt(1 - 4x^2)) ; [0, 0.5)<br />y = (1/2)(sqrt(-(2x - 3)*(2x - 1)) + 1) ; [0.5, 1]<br />

- OPfloat OPtween_exponentialEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = 2^(10(x - 1))<br />

- OPfloat OPtween_exponentialEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = -2^(-10x) + 1<br />

- OPfloat OPtween_exponentialEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)2^(10(2x - 1)) ; [0,0.5)<br />y = -(1/2)*2^(-10(2x - 1))) + 1 ; [0.5,1]<br />

- OPfloat OPtween_elasticEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = sin(13pi/2*x)*pow(2, 10 * (x - 1))<br />

- OPfloat OPtween_elasticEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = sin(-13pi/2*(x + 1))*pow(2, -10x) + 1<br />

- OPfloat OPtween_elasticEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)*sin(13pi/2*(2*x))*pow(2, 10 * ((2*x) - 1)) ; [0,0.5)<br />y = (1/2)*(sin(-13pi/2*((2x-1)+1))*pow(2,-10(2*x-1)) + 2) ; [0.5, 1]<br />

- OPfloat OPtween_backEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = x^3-x*sin(x*pi)<br />

- OPfloat OPtween_backEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function : y = 1-((1-x)^3-(1-x)*sin((1-x)*pi))<br />

- OPfloat OPtween_backEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tweening Function :<br />y = (1/2)*((2x)^3-(2x)*sin(2*x*pi)) ; [0, 0.5)<br />y = (1/2)*(1-((1-x)^3-(1-x)*sin((1-x)*pi))+1) ; [0.5, 1]<br />

- OPfloat OPtween_bounceEaseOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tween Function : Bounce at Hard Preset Points<br />

- OPfloat OPtween_bounceEaseIn ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tween Function : Bounce Backwards at Hard Preset Points<br />

- OPfloat OPtween_bounceEaseInOut ( OPfloat p )

.. epigraph::
	.. raw:: html

		Tween Function : Bounce at Hard Preset Points<br />
