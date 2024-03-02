The equation for a reflection across a line an angle $\phi$ from the x axis is
$$Ref_{\phi}(x) = (2M_{proj_{\phi}}-I)\vec{x}$$
Thus, the transformation matrix $M_{Ref_{\phi}}$ is
$$M_{Ref_{\phi}} = 2M_{Proj_{\phi}}-I$$

To reflect across a plane, it is a little different:

For ex., if we have the plane $x+y+z = 1$
We use the projection for $\vec{x_{\perp}}$ instead of $\vec{x_{\parallel}}$
Thus, $Ref_{p}\vec{x}$ =
$$\vec{x}-2\vec{x_{\perp}}$$
$$M_{Proj_{p}} = I - M_{Proj_{\hat{n}}}$$
$$M_{Proj_{p}} = I - 2M_{Proj_{\hat{n}}}$$
 