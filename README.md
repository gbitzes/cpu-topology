cpu-topology
============

A small script to view the topology of the CPUs.
Running ./cpu-topology.py will give a breakdown based on socket, NUMA node, core, and hardware thread on the current machine.

Sometimes it's useful to pin processes to specific cores; one way to do it is by placing the proesses as "far away" as possible. In this case, you continuously alternate between sockets, nodes, cores and threads.

Another one is to place them as close together as possible. In this case, you completely fill each hardware thread, core, node, and socket, before proceeding to the next.

When a machine has many cores, it's often tedious to make such a mapping by hand. You can generate such an affiniy mapping by running "./cpu-topology.py scatter|compact"

<sub><sup>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</sup></sub>
