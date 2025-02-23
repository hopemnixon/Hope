<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Hope Nixon the Agent - Buyer Questionnaire</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      margin: 0;
      padding: 0;
      color: #333;
    }
    .container {
      max-width: 800px;
      margin: 30px auto;
      background: #fff;
      padding: 20px 40px;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }
    header {
      text-align: center;
      margin-bottom: 20px;
    }
    header h1 {
      color: #007BFF;
    }
    h2 {
      text-align: center;
      margin-bottom: 20px;
    }
    .section {
      margin-bottom: 20px;
    }
    label {
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }
    input[type="text"],
    input[type="email"],
    input[type="date"],
    input[type="number"],
    textarea,
    select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    textarea {
      resize: vertical;
    }
    .checkbox-group label {
      display: inline-block;
      margin-right: 15px;
      font-weight: normal;
    }
    .submit-button {
      background-color: #007BFF;
      color: #fff;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-size: 16px;
      margin-top: 20px;
    }
    .submit-button:hover {
      background-color: #0056b3;
    }
    .footer {
      text-align: center;
      margin-top: 30px;
      font-style: italic;
      font-size: 1.1em;
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Hope Nixon the Agent</h1>
      <h2>Buyer Questionnaire</h2>
    </header>
    
    <form id="buyerForm">
      <!-- Section 1: Basic Information -->
      <div class="section">
        <h3>Basic Information</h3>
        <label for="fullName">Full Name:</label>
        <input type="text" id="fullName" name="fullName" required>
        
        <label for="contactInfo">Contact Information (Phone & Email):</label>
        <input type="text" id="contactInfo" name="contactInfo" required>
        
        <label for="currentResidence">Current Residence:</label>
        <input type="text" id="currentResidence" name="currentResidence">
        
        <label for="moveInDate">Desired Move-In Date:</label>
        <input type="date" id="moveInDate" name="moveInDate">
      </div>
      
      <!-- Section 2: Current Situation & Motivation -->
      <div class="section">
        <h3>Current Situation & Motivation</h3>
        <label>Primary Reasons for Moving (check all that apply):</label>
        <div class="checkbox-group">
          <label><input type="checkbox" name="reasons" value="Need more space"> Need more space</label>
          <label><input type="checkbox" name="reasons" value="Downsizing"> Downsizing</label>
          <label><input type="checkbox" name="reasons" value="Job relocation"> Job relocation</label>
          <label><input type="checkbox" name="reasons" value="Change in neighborhood"> Change in neighborhood</label>
          <label><input type="checkbox" name="reasons" value="Lifestyle change"> Lifestyle change (e.g., closer to amenities, quieter area)</label>
          <label><input type="checkbox" name="reasons" value="Other"> Other (please specify below)</label>
        </div>
        <label for="otherReason">If Other, please specify:</label>
        <input type="text" id="otherReason" name="otherReason">
        
        <label for="mainMotivation">Describe Your Main Motivation:</label>
        <textarea id="mainMotivation" name="mainMotivation" rows="3" required></textarea>
      </div>
      
      <!-- Section 3: Property Requirements & Preferences -->
      <div class="section">
        <h3>Property Requirements & Preferences</h3>
        <label for="propertyType">Type of Property Sought:</label>
        <select id="propertyType" name="propertyType">
          <option value="Single-family home">Single-family home</option>
          <option value="Condo">Condo</option>
          <option value="Townhouse">Townhouse</option>
          <option value="Other">Other</option>
        </select>
        
        <label for="bedrooms">Bedrooms Needed:</label>
        <input type="number" id="bedrooms" name="bedrooms" min="0">
        
        <label for="bathrooms">Bathrooms Needed:</label>
        <input type="number" id="bathrooms" name="bathrooms" min="0">
        
        <label for="mustHaveFeatures">Top Three Must-Have Features:</label>
        <textarea id="mustHaveFeatures" name="mustHaveFeatures" rows="3" placeholder="e.g., modern kitchen, outdoor space, updated fixtures"></textarea>
        
        <label for="preferredLocation">Preferred Neighborhood/Area:</label>
        <input type="text" id="preferredLocation" name="preferredLocation">
        
        <label for="locationAttraction">What Attracts You to This Area?</label>
        <textarea id="locationAttraction" name="locationAttraction" rows="3" placeholder="Consider aspects like schools, safety, amenities, commute, etc."></textarea>
      </div>
      
      <!-- Section 4: Budget & Financial Considerations -->
      <div class="section">
        <h3>Budget & Financial Considerations</h3>
        <label for="budget">Budget Range or Maximum Budget:</label>
        <input type="text" id="budget" name="budget" placeholder="e.g., $300,000 - $500,000">
        
        <label>Are you pre-approved for a mortgage?</label>
        <label><input type="radio" name="mortgageStatus" value="Yes" required> Yes</label>
        <label><input type="radio" name="mortgageStatus" value="No" required> No</label>
        
        <label for="budgetFlexibility">Would you be willing to stretch your budget for a property that perfectly meets your must-have features?</label>
        <select id="budgetFlexibility" name="budgetFlexibility">
          <option value="Yes">Yes</option>
          <option value="No">No</option>
          <option value="Maybe">Maybe (please explain in additional comments below)</option>
        </select>
      </div>
      
      <!-- Section 5: Lifestyle & Long-Term Considerations -->
      <div class="section">
        <h3>Lifestyle & Long-Term Considerations</h3>
        <label for="duration">Expected Duration of Stay:</label>
        <input type="text" id="duration" name="duration" placeholder="e.g., 5 years, 10+ years">
        
        <label for="neighborhoodType">What type of neighborhood do you envision? (e.g., quiet and residential, vibrant and urban, family-friendly)</label>
        <input type="text" id="neighborhoodType" name="neighborhoodType">
        
        <label for="lifestyleAmenities">Are there any amenities (e.g., parks, gyms, transit, cultural centers) that are especially important to you?</label>
        <textarea id="lifestyleAmenities" name="lifestyleAmenities" rows="3"></textarea>
      </div>
      
      <!-- Section 6: Trade-Offs and Flexibility -->
      <div class="section">
        <h3>Trade-Offs and Flexibility</h3>
        <label for="priorityTradeOff">If forced to choose, would you prefer a prime location or additional space/features? Please explain your reasoning:</label>
        <textarea id="priorityTradeOff" name="priorityTradeOff" rows="3"></textarea>
        
        <label for="willingnessCompromise">Which property aspects could you be flexible about? (e.g., property age, interior finishes, outdoor space, storage/utility space)</label>
        <textarea id="willingnessCompromise" name="willingnessCompromise" rows="3" placeholder="Please indicate your level of flexibility for each"></textarea>
        
        <label for="dealBreakers">Are there any features or issues that would be a deal-breaker for you?</label>
        <textarea id="dealBreakers" name="dealBreakers" rows="3"></textarea>
      </div>
      
      <!-- Section 7: Final Comments -->
      <div class="section">
        <h3>Additional Information</h3>
        <label for="additionalInfo">Please share any other details or preferences that could help me better understand your needs:</label>
        <textarea id="additionalInfo" name="additionalInfo" rows="3"></textarea>
      </div>
      
      <button type="submit" class="submit-button">Submit</button>
    </form>
    
    <div id="thankYouMessage" class="footer" style="display: none;">
      <p>Thank you for filling out the questionnaire. I greatly appreciate your time and I will look these over and get back to you <3</p>
    </div>
  </div>
  
  <script>
    // Basic form submission handling to display thank you message
    document.getElementById('buyerForm').addEventListener('submit', function(event) {
      event.preventDefault();
      this.style.display = 'none';
      document.getElementById('thankYouMessage').style.display = 'block';
      // Here, you could also add AJAX code to send the form data to your server.
    });
  </script>
</body>
</html>
