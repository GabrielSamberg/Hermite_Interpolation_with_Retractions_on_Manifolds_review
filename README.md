# Hermite Interpolation with Retractions on Manifolds paper review
In the field of Riemannian optimization (optimization problems on Riemannian manifolds) the paper is focusing on an interpolation problem of data samples that are laying on some Riemannian manifold. In this specific setting, the data samples have a prescribed tangent vector at each data point. The demand is that the interpolant is a curve contained in the manifold that interpolates the data points and matches the prescribed derivatives at each point and in addition is globally continuously differentiable.
Such problem is called Hermite interpolation problem generalized to Riemannian manifolds.
In order to solve this problem one can think to use the exponential map (the geodesic endpoint curves induced by it) and it's inverse, the logarithmic map. An evident shortcoming of such an approach is that in many cases it is not obvious that there exist a computationally efficient way of computing the exponential map or its inverse. To address this drawback the paper suggests the usage of a broader family of manifold curves that are induced by a family of manifold valued functions called retractions.
This family of curves is used by the authors in a generalization proposed by them to an algorithm which was originally designed for the Euclidean space. In the Euclidean setting, given two points, the original algorithm constructs a polynomial curve between them, the algorithm is called de Casteljau algorithm and the authors are generalizing it to manifolds and retraction endpoint curves in order to solve the Hermite interpolation problem on Riemannian manifolds.

Here is my [detailed review](./Hermite_interpolation_with_retractions_on_manifolds_review-3.pdf) of the mathematical framework of the paper.

Below you can find the Colab notebook containing the implementation detail of one of the examples discussed in the paper.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/GabrielSamberg/Hermite_Interpolation_with_Retractions_on_Manifolds_review/blob/main/Hermite_interpolation.ipynb
)
