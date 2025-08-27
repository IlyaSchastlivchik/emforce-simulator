[Русская версия](README_RU.md) | [English version](README.md)

# EMForce Simulator: Electromagnetic Interaction Modeling

![Electromagnetic Field Visualization](images/field_simulation.png)

## 🚀 About the Project

An innovative platform for simulating electromagnetic interactions that combines:
- Dynamic modeling of Lorentz and Ampere forces
- AI integration (DeepSeek) for calculations
- Visualization on the Unity engine
- Static field calculations through FEMM

## ✨ Key Features

- **Real-time simulations** of electromagnetic phenomena
- **AI-assisted design** of electronic circuits
- **Seamless integration** between Unity, FEMM and AI components
- **Export capability** to LTSpice and other formats
- **Interactive 3D visualization** of field interactions

## 🛠 Technology Stack

| Component | Technologies |
|-----------|-------------|
| Graphics Interface | Unity, HLSL, URP |
| Physics Engine | Custom C# Lorentz Force engine |
| Field Calculations | FEMM integration, Python scripts |
| AI Component | DeepSeek API, PyTorch |
| Visualization | Shader Graph, Compute Shaders |

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/emforce-simulator.git
cd emforce-simulator

# Install dependencies
pip install -r requirements.txt

# Run demo simulation
python demo_simulation.py

## 🧪 Example Usage

```python
# Lorentz force calculation
def lorentz_force(q, E, v, B):
    """Calculate Lorentz force"""
    return q * (E + np.cross(v, B))

# Example parameters
charge = 1.6e-19  # C
electric_field = np.array([0, 0, 0])  # V/m
velocity = np.array([1e6, 0, 0])  # m/s
magnetic_field = np.array([0, 0, 1e-3])  # T

force = lorentz_force(charge, electric_field, velocity, magnetic_field)
print(f"Lorentz force: {force} N")
 ```

## 📊 Project Structure

 ```
 emforce-simulator/
 ├── src/                 # Source code
 │   ├── unity/           # Unity project files
 │   ├── femm/            # FEMM integration scripts
 │   └── ai/              # AI assistant module
 ├── docs/                # Documentation
 ├── simulations/         # Example simulations
 ├── images/              # Graphics and diagrams
 └── README.md            # This file
 ```
 
 
## 🤝 Contributing

We welcome contributions in areas such as:
- Development of physical models
- Electromagnetic field visualization
- Integration with additional simulators
- Algorithm optimization

Please read our [contributing guidelines](docs/CONTRIBUTING.md) for details.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

EN [rattchanel@gmail.com](mailto:rattchanel@gmail.com)
RU [tesla2you@mail.ru](mailto:tesla2you@mail.ru)

Project Link: [https://github.com/IlyaSchastlivchik/emforce-simulator](https://github.com/IlyaSchastlivchik/emforce-simulator)

---

*Developed with [DeepSeek](https://deepseek.com) and [Unity](https://unity.com)*