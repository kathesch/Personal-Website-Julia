@def title = "Katherine Gruenewald - Animations"
@def hasmath = false
@def hascode = true


\newcommand{\mtt}[2]{
  ~~~
<figure style="text-align:center;border: thin silver solid;">
<img src="!#1" style="width:100%"/>
<figcaption>#2
</figure>
~~~
}

# Gallery

## Fast poisson solver using Euler-Poisson-Darboux Equation

\mtt{/assets/plot_676.gif}{Figure 1: Comparison of EPD Eq. with a explict solver of the heat eq.}

## Interactive stress-strain curve

We can model a simple polymer material with molecular dynamics and interactively output coordinates to Makie. 


\mtt{/assets/nvearinter (1).gif}{Figure 1: Basic initialization}

 
\mtt{/assets/stretchpolymer.gif}{Figure 2: Stretching}
\mtt{/assets/compresspolymer.gif}{Figure 3: Compression}

## Bee swarm image interpolation and modal analysis

\mtt{/assets/beeeinterpolation.gif}{Figure 1: Image analysis fitting a video of a bee swarm scattering to a 3D model.}

\mtt{/assets/beeeigenmodes.gif}{Figure 2: Computing vibrational modes of a bee swarm model ordered by energy (lowest to highest). }


## Lotka-Volterra network modelling

\mtt{/assets/biomassflowlabeled.gif}{Figure 1: Simple graphic showing flow of biomass in a lotka-voltera network}

\mtt{/assets/biomassflownetwork.gif}{Figure 2: Biomass flow in a more complicated lotka-voltera network}

\mtt{/assets/neuralnet.gif}{Figure 3: Neural network controlling one organism's population to prevent extinction of organisms in other nodes of the network. }

## Eigenmodes of vibrations for simple geometries

\mtt{/assets/lowest.gif}{Figure 1: Lowest order vibrational modes for a 2d plane bounded at its edges.}

\mtt{/assets/2ndeigenmode.gif}{Figure 2: 2nd lowest vibrational mode for the above plane.}

\mtt{/assets/3deigen.gif}{Figure 3: A volumetric vibrational mode in a cube.}


<!--
# Code generation

**Note: this feature is experimental and the API might change frequently**

`toexpr(ex)` turns any expression (`ex`) into the equivalent `Expr` which is suitable for `eval`. The `SymbolicUtils.Code` module provides some combinators which provides the ability to construct more complex expressions than just function calls. These include:



- Let blocks
- Functions with arguments and keyword arguments
  - Functions with arguments which are to be de-structured
- Expressions that set array elements in-place
- Expressions that create an array similar in type to a reference array (currently supports `Array`, `StaticArrays.SArray`, and `LabelledArrays.SLArray`)
- Expressions that create sparse arrays

**Do `using SymbolicUtils.Code` to get the following bindings**

## `toexpr`

{{doc toexpr toexpr fn Code}}

## Code Combinators

These are all exported when you do `using SymbolicUtils.Code`

{{doc Assignment Assignment type Code}}

{{doc Let Let type Code}}

{{doc Func Func type Code}}

{{doc SpawnFetch SpawnFetch type Code}}

{{doc SetArray SetArray type Code}}

{{doc MakeArray MakeArray type Code}}

{{doc MakeSparseArray MakeSparseArray type Code}}

{{doc MakeTuple MakeTuple type Code}}

{{doc LiteralExpr LiteralExpr type Code}}
-->