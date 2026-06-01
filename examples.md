# Examples

## Defining a Material

```carp
(use Material)
(use Vector3)

(let [iron (Material.make (Vector3.init 0.56 0.57 0.58) 0.1 1.0)]
  (do-something-with iron))
```

## Using Shading.blinn-phong

```carp
(use Shading)
(use Vector3)

(let [n (Vector3.init 0.0 1.0 0.0)
      l (Vector3.normalize (Vector3.init 1.0 1.0 1.0))
      v (Vector3.init 0.0 0.0 1.0)
      albedo (Vector3.init 1.0 0.0 0.0)
      roughness 0.2
      metallic 0.0]
  (Shading.blinn-phong n l v albedo roughness metallic))
```
