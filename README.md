# bitter

### Bitslicer for bytes 
```go

$ go doc -all -u bitter

package bitter // import "github.com/futzu/bitter"


TYPES

type Bitn struct {
        idx  uint
        bits string
}
    Bitn converts bytes to a list of bits.

func (b *Bitn) As90k(bitcount uint) float64
    As90k is AsFloat / 90000.00

func (b *Bitn) AsBool() bool
    AsBool slices 1 bit and returns true for 1 , false for 0

func (b *Bitn) AsDeHex(bitcount uint) []byte
    AsDeHex slices bitcount of bits and returns as hex string

func (b *Bitn) AsFloat(bitcount uint) float64
    AsFloat slices bitcount of bits and returns as float64

func (b *Bitn) AsHex(bitcount uint) string
    AsHex slices bitcount of bits and returns as hex string

func (b *Bitn) AsUInt64(bitcount uint) uint64
    AsUInt64 is a wrapper for Chunk

func (b *Bitn) Chunk(bitcount uint) uint64
    Chunk slices bitcount of bits and returns it as a uint64

func (b *Bitn) Forward(bitcount uint)
    Forward advances b.idx by bitcount

func (b *Bitn) Load(bites []byte)
    Load raw bytes and convert to bits


```
