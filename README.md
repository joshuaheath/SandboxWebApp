using System.ComponentModel.DataAnnotations;

namespace SandboxWebApp.Models
{
    public class Trail
    {
        public int ID { get; set; }
        [StringLength(100)]
        [Required]
        public string Title { get; set; } = string.Empty;

        [StringLength(500)]
        [Required]
        public string Description { get; set; } = string.Empty;
        [Required]
        public int Length {  get; set; }
        [Required]
        public int ElevationGain { get; set; }
        [Required]
        public double EstimatedTime { get; set; }
        [Required]
        public string Difficulty { get; set; } = string.Empty;
        [Required]
        public string ImageFilename { get; set; } = string.Empty;
        [Required]
        public DateTime CreatedDate { get; set; } = DateTime.Now;
    }
}
