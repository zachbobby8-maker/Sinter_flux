# FLUX_GRAMMAR.md - The Grammar & Syntax Manual

## 1. THE .flux FILE FORMAT
Fluid Script (`.flux`) is not a procedural language; it is a **Declarative Manifold Definition**. Instead of functions, we define **Braids**. Instead of variables, we define **Pulses**.

## 2. BASIC SYNTAX

### The Braid Definition
A Braid is a logic unit that persists in the Lattice.
```flux
braid LatticeSync {
    input manifold user_intent;
    input manifold zone_state;
    
    // Resonance logic
    resonate(user_intent, 0.85);
    
    // Interlacing two manifolds
    output braid result = interlace(user_intent, zone_state);
}
```

### Pulses (Events)
Pulses are short-lived data ripples.
```flux
pulse OnAuthSuccess {
    target: "sinter_login";
    action: PHASE_SHIFT(0.5);
}
```

## 3. KEYWORDS
- `manifold`: A multi-dimensional data structure.
- `shimmer`: A function that adds pseudo-randomness (entropy).
- `vortex`: Compresses data for transmission.
- `phase`: Shifts the timing of a pulse.
- `lock`: Ensures the manifold stays stable in the local zone.

---

# BRAID_KIT.md - The Standard Library

## 1. NETWORKING (`net.flux`)
- `net.ripple(manifold)`: Broadcasts a manifold to the local Resonance Zone.
- `net.phase_lock(address)`: Establishes a peer-to-peer sync.

## 2. CRYPTOGRAPHY (`crypt.flux`)
- `crypt.braid_hash(manifold)`: Creates a signature based on the manifold's wave geometry.
- `crypt.lattice_seal(manifold, key)`: Encrypts data using local lattice entropy.

## 3. RENDERING (`ui.flux`)
- `ui.glitch(element, intensity)`: Applies a visual shimmer to a UI component.
- `ui.project_vortex(canvas_id)`: Renders the active execution state.

---

# ARCHITECT_GUIDE.md - Best Practices

1. **Avoid Noise:** Do not resonate manifolds with low integrity (< 0.5). It creates "Harmonic Noise" that slows down the local zone.
2. **Phase Timing:** Always align your pulses with the 39.42 kHz Sync Pulse.
3. **Lattice Respect:** Free up unused manifold space. The Lattice is a shared resource.
