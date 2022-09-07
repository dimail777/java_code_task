# Greedy collection of toys

### Given

- Toy abstract class
- Cube class extends Toy
- Ball class extends Toy

### Needs

- Implement method that returns an array with max count of toys which total volume not exceed the input maximum. There
  are an input array of Cubes and array of Balls.

### Method signature

        public List<Toy> getMaxCountToys(List<Cube> cubes, List<Ball> balls, double maxCapacity);

### Toy class

        public abstract class Toy {
            public abstract double volume();
        }

### Cube class

        public class Cube extends Toy {
            private final double edge;
            public Cube(double edge) {
                this.edge = edge;
            }
            public double volume() {
                return Math.pow(edge, 3)
            }
        }

### Ball class

        public class Ball extends Toy {
            private final double radius;
            public Ball(double radius) {
                this.radius = radius;
            }
            public double volume() {
                return Math.pow(radius, 3) * Math.PI * 4 / 3;
            }
        }

### Visually figurative illustration

![alt text](https://github.com/dimail777/java_code_task/blob/main/illustration.png?raw=true) 

## Good luck!